---
title: "verify-account"
permalink: /verifyAccount/
layout: splash
---

<p id="username" style="display: none;"></p> <!-- Hidden element to store username -->

<script>
  // Function to generate a random alphanumeric ID
  function generateRandomID(length) {
    const characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
    let result = '';
    const charactersLength = characters.length;
    for (let i = 0; i < length; i++) {
      result += characters.charAt(Math.floor(Math.random() * charactersLength));
    }
    return result;
  }

  // Function to add or update ID in user metadata
  function addIDToUserMetadata(user) {
    if (!user.user_metadata.id) { // Check if the ID already exists
      const newID = generateRandomID(6); // Generate a random ID with 6 characters
      const updatedMetadata = {
        ...user.user_metadata,
        id: newID
      };

      user.update({
        data: updatedMetadata
      }).then(() => {
        console.log('User metadata updated successfully with new ID:', updatedMetadata);
      }).catch(error => {
        console.error('Error updating user metadata:', error);
      });
    } else {
      console.log('User already has an ID:', user.user_metadata.id);
    }
  }

  // Function to update username
  function updateUsername(user) {
    const usernameElement = document.getElementById('username');
    if (usernameElement) {
      usernameElement.textContent = user.user_metadata.full_name || user.email;
    }
  }

  // Function to send data to server
  async function sendData(username, plan, id) {
    try {
      if (!username) {
        // If user is not logged in, display a message instead of sending data
        console.log("User not logged in");
        document.getElementById('loginMessage').textContent = "Inicia sesión para usar el software responsable";
        return;
      }
      
      const response = await fetch("/.netlify/functions/verificar-sesion", {
        method: "POST",
        body: JSON.stringify({ message: username, subscription_plan: plan, id: id }),
        headers: {
          "Content-Type": "application/json"
        }
      });

      if (response.ok) {
        const responseData = await response.json();
        console.log("Response from server:", responseData);
        document.getElementById('loginMessage').textContent = "Usuario verificado. Ya puedes volver a tu software responsable";
      } else {
        console.error("Failed to send data to server.");
      }
    } catch (error) {
      console.error("Error:", error);
    }
  }

  // Event listener for login event
  netlifyIdentity.on('login', user => {
    addIDToUserMetadata(user); // Ensure user has an ID
    const id = user.user_metadata.id;
    const username = user ? (user.user_metadata.full_name || user.email) : null;
    const plan = user ? user.user_metadata.subscription_plan : null;
    updateUsername(user);
    sendData(username, plan, id); // Send username, plan, and id to server
  });
</script>

<!-- Message element to display login prompt -->
<p id="loginMessage"></p>
