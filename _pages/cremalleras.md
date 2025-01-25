---
title: "Cremalleras"
permalink: /cremalleras/
layout: default
---



<div class="splash-container">
  <!-- Full-width background image -->
  <img src="/assets/images/aulamatinal.png" alt="Full Width Image" class="splash-image">

  <!-- Grey transparent background image -->
  <div class="grey-background"></div>

  <!-- Text title at top right -->
  <div class="top-left">Aula matinal</div>

  <!-- Right image upfront -->
  <img src="/assets/images/niñacomiendo.png" alt="Right Image" class="right-image">

  <!-- Text content at bottom left -->
  <div class="bottom-left">
    <p>JAPONEDUCA, parte del GRUPO JAPÓN, ofrece servicios educativos, ocio y tiempo libre. Nuestro programa incluye aula matinal adaptada a horarios familiares, fortaleciendo la autonomía escolar bajo el Plan de Apertura de Centros en Andalucía.</p>
    <button class="plan-button2" onclick="location.href='https://app.grupojapon.es/index.php/registro'" style="font-weight: 700;">INSCRÍBETE</button>
  </div>
</div>


<style>
  .splash-container {
    position: relative;
    width: 100%;
    max-width: none;
    overflow: hidden;
    margin-bottom: 3em;
    padding: 0;
    padding-top: 3.5em;
    margin-top: 2em;
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* Default: 2 columns */
    grid-template-rows: 142px 1fr; /* Default: 2 rows */
    grid-column-gap: 20px; /* Adjust spacing between columns */
    grid-row-gap: 20px; /* Adjust spacing between rows */
    align-items: end;
  }

  /* Styling for the right image */
  .right-image {
    grid-row: 1 / 3; /* Both rows */
    grid-column: 2 / 3; /* Default: second column */
    width: 370px;
    z-index: 10; /* Ensure above background image */
    margin: 0 auto;
    transform: translateX(calc(-50% + 80px));
  }

  .grey-background {
    background-color: rgba(127, 127, 127, 0.7); /* Semi-transparent grey */
    position: absolute; /* Ensures it stays within the container */
    top: 0;
    left: 0;
    width: 55%; /* Occupy the left half of the splash container */
    height: 100%; /* Full height of the splash container */
    z-index: 5; /* Below the text but above the background image */
    margin-top: 3.5em;
    transform: translateX(-80px);
  }

  .bottom-left {
    z-index: 10;
    max-width: 650px;
    text-align: left;
    margin-left: auto;
    margin-right: 1em;
    color: white;
    padding: 20px;
    align-self: start;
  }

  .top-left {
    grid-row: 1 / 2; /* First row */
    grid-column: 1 / 2; /* Now in the first column */
    font-size: 42px;
    font-weight: 700;
    color: white;
    z-index: 10; /* Ensure above background image */
    text-align: left;
    margin-right: 8.8em;
    margin-left: auto;
    padding-left: 20px;
  }

  /* Breakpoint for smaller screens: 1 column, 3 rows */
  @media (max-width: 967px) {
    .splash-container {
      grid-template-columns: 1fr; /* 1 column */
      grid-template-rows: repeat(3, auto); /* 3 rows */
      grid-row-gap: 0px; /* Adjust row spacing */
      margin-top: 0;
    }

    /* Adjust the right image to fit in the first column (stacked layout) */
    .right-image {
      grid-row: 2 / 3; /* Place the image in the second row */
      grid-column: 1 / 2; /* Place it in the first column */
      width: 250px; /* Make it responsive */
      transform: none;
    }

    /* Adjust the grey background to occupy the last row */
    .grey-background {
      position: static; /* Remove absolute positioning */
      grid-row: 3 / 3; /* Place it in the last row */
      grid-column: 1 / 2; /* Full width of the single column */
      width: 100%; /* Full width of the column */
      height: 100%; /* Adjust height automatically */
      transform: none; /* Remove the horizontal transform */
    }

    .bottom-left {
      z-index: 10;
      text-align: left;
      color: white;
      padding: 20px;
      align-self: start;
      grid-column: 1 / 1;
      grid-row: 3 / 3;
    }

    .top-left {
      grid-row: 1 / 2; /* First row */
      grid-column: 1 / 2; /* Now in the first column */
      font-size: 34px;
      font-weight: 700;
      color: white;
      z-index: 10; /* Ensure above background image */
      text-align: left;
      margin-right: 0;
      margin-left: 0;
      padding-left: 20px;
    }
  }

  .splash-image {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    object-fit: cover;
    z-index: -1;
    margin: 0;
  }

  .bottom-left p {
    font-size: 17px;
    margin-bottom: 3em;
  }

  .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
    margin-top: 2em;
  }

  .product {
    background: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 12px;
    text-align: center;
    padding: 15px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    display: flex;
    flex-direction: column;
    justify-content: space-between; /* Ensures consistent positioning */
    height: 100%; /* Makes all cards the same height */
  }

  .product:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
  }

  .product img {
    max-width: 100%;
    height: auto;
    border-radius: 12px;
    margin: 0 auto; /* Ensures the image is horizontally centered */
  }

  .product h3 {
    font-size: 20px;
    color: #333;
    margin: 10px 0 5px; /* Adds spacing above and below */
  }

  .product p {
    font-size: 16px;
    color: #666;
    line-height: 1.5;
    margin: 0; /* Ensures it stays close to the title */
  }
</style>




<div class="product-grid">
  <div class="product">
    <img src="/assets/images/cremallera1.png" alt="Product 1">
    <h3>Producto 1</h3>
    <p>Breve descripción del producto 1.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera2.png" alt="Product 2">
    <h3>Producto 2</h3>
    <p>Breve descripción del producto 2.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera3.png" alt="Product 3">
    <h3>Producto 3</h3>
    <p>Breve descripción del producto 3.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera4.png" alt="Product 4">
    <h3>Producto 4</h3>
    <p>Breve descripción del producto 4.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera5.png" alt="Product 5">
    <h3>Producto 5</h3>
    <p>Breve descripción del producto 5.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera6.png" alt="Product 6">
    <h3>Producto 6</h3>
    <p>Breve descripción del producto 6.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera7.png" alt="Product 7">
    <h3>Producto 7</h3>
    <p>Breve descripción del producto 7.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera8.png" alt="Product 8">
    <h3>Producto 8</h3>
    <p>Breve descripción del producto 8.</p>
  </div>
  <div class="product">
    <img src="/assets/images/cremallera9.png" alt="Product 9">
    <h3>Producto 9</h3>
    <p>Breve descripción del producto 9.</p>
  </div>
</div>







<div style="text-align:center; margin-top:7em">
  ¿Dudas? No te las guardes, pregúntanos.
</div>

<form name="contact" action="/_pages/success.html" method="POST" data-netlify="true" class="contact-form">
  <input type="hidden" name="subject" id="subject" value="Mensaje de (nombre)" />
  
  <p>
    <label for="name">Nombre:</label><br />
    <input type="text" id="name" name="name" required />
  </p>
  
  <p>
    <label for="email">Correo Electrónico:</label><br />
    <input type="email" id="email" name="email" required />
  </p>
  
  <p>
    <label for="phone">Teléfono:</label><br />
    <input type="tel" id="phone" name="phone" required />
  </p>
  
  <p>
    <label for="message">Mensaje:</label><br />
    <textarea id="message" name="message" rows="5" required></textarea>
  </p>
  
  <p style="text-align: center;">
    <button type="submit" class="submit-button">Enviar</button>
  </p>
</form>

<script>
  document.querySelector('form').addEventListener('submit', function(event) {
    var name = document.getElementById('name').value;
    var phone = document.getElementById('phone').value;
    var subjectField = document.getElementById('subject');
    subjectField.value = `Mensaje de ${name} - Teléfono: ${phone}`;
  });
</script>


<style>
.plans-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

.plan {
  width: 400px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background: white;
  text-align: center;
  margin: 60px 12px;
  text-decoration: none;
  color: inherit;
  transition: background-color 0.3s ease, box-shadow 0.3s ease;
}

.plan:hover {
  background-color: #f0f0f0;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  text-decoration: none;
}

.plan h2, .plan p {
  color: inherit;
}

.contact-form {
  max-width: 600px;
  margin: 0 auto;
  text-align: left;
}

.faq-container {
  width: 100%;
  max-width: 41rem;
  margin: 4em auto;
  text-align: left;
}

.accordion {
  background-color: transparent !important;
  outline: 0 !important;
  width: 100%;
  padding: 20px;
  text-align: left;
  border: none;
  cursor: pointer;
  line-height: 40px;
  background-color: transparent;
  color: black; /* Ensure it's the same color as the rest of the text */
  outline: none;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-top: 1px solid #ccc;
  font-family: inherit; /* Inherit the same font as the rest of the text */
  font-size: 17px; /* Set the same size as the answer text */
  font-weight: normal; /* Ensure consistent font weight */
}

.accordion-icon {
  transition: transform 0.3s ease;
}

.accordion-icon.rotated {
  transform: rotate(180deg);
}

.panel {
  font-size: 17px;
  padding: 0 18px;
  height: 0;
  overflow: hidden;
  transition: height 0.3s ease;
}

.panel.open {
  height: auto;
}

.plan-button:hover {
  background-color: #9b1b20;
}

.submit-button {
  background-color: rgb(69 28 72);
  color: white;
  border: none;
  padding: 15px 100px;
  margin: 40px;
  text-align: center;
  font-size: 20px;
  border-radius: 5px;
  cursor: pointer;
}

.submit-button:hover {
  background-color: #9b1b20;
}
</style>

<script>
  var accordions = document.querySelectorAll(".accordion");

  accordions.forEach(function(accordion) {
    accordion.addEventListener("click", function() {
      this.classList.toggle("active");
      var icon = this.querySelector(".accordion-icon");
      icon.classList.toggle("rotated");

      var panel = this.nextElementSibling;
      if (panel.style.height) {
        panel.style.height = null;
      } else {
        panel.style.height = panel.scrollHeight + "px";
      }
    });
  });
</script>




<style>
  .table-container {
    margin-top: 30px; /* Ajusta el margen superior según sea necesario */
  }

  .table-container table {
    border-collapse: collapse;
    border: none; /* elimina los bordes de la tabla */
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .table-container td {
    padding: 8px;
    border: 1px solid #ccc;
    text-align: left;
  }

  .table-container th {
    padding: 8px;
    background-color: transparent !important; /* Fondo transparente */
    border: none; /* Sin bordes */
  }

  .table-container thead th {
    background-color: transparent !important; /* Fondo transparente */
  }

  .table-container tbody tr:nth-child(even) {
    background-color: #e7e7e7; /* Cambia el color de fondo para las filas pares */
  }

  /* Elimina los bordes de las celdas exteriores */
  .table-container th:first-child,
  .table-container td:first-child {
    border-left: none;
  }

  .table-container th:last-child,
  .table-container td:last-child {
    border-right: none;
  }

  /* Elimina la última línea horizontal */
  .table-container tr:last-child th,
  .table-container tr:last-child td {
    border-bottom: none;
  }

  /* Elimina la primera línea horizontal */
  .table-container tr:first-child th,
  .table-container tr:first-child td {
    border-top: none;
  }

  /* Elimina la segunda línea horizontal */
  .table-container tr:nth-child(2) th,
  .table-container tr:nth-child(2) td {
    border-top: none;
  }
</style>
