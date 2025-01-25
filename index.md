---
#title: "Ciclos de FP oficiales en grupos reducidos y servicios educativos"
title: "La esencia del flamenco en cada paso"
layout: splash
header:
  overlay_image: /assets/images/page-header-teaser.png
  #overlay_filter: rgba(102,153,255,0.5)
  actions:
    - label: "Solicita información"
      url: "https://japonformacion.netlify.app/contacto/"
excerpt: "Aprende y siente el flamenco con clases auténticas y espectáculos inolvidables"
---


<div class="plans-container">
  <a href="/aula_matinal" class="plan">
    <h2>Aula Matinal</h2>
    <p>JAPONEDUCA ofrece aula matinal en colegios, brindando a los alumnos un espacio seguro y enriquecedor para comenzar el día, facilitando además la organización de las familias.</p>
  </a>

  <a href="/aula_espera" class="plan">
    <h2>Aula de Espera</h2>
    <p>JAPONEDUCA ofrece un servicio de aulas de espera en colegios, proporcionando un espacio seguro y supervisado para los alumnos, adaptándose a las necesidades familiares y escolares.</p>
  </a>

  <a href="/judo" class="plan">
    <h2>Judo</h2>
    <p>Desde 1994, JAPONSPORT promueve el judo en Huelva para fomentar hábitos saludables y mejorar la calidad de vida.</p>
  </a>

  <a href="/FPSuperior" class="plan">
    <h2>Grados Superiores</h2>
    <p>Accede con el título de Bachillerato, una FP de Grado Medio o Superior o mediante prueba de acceso.</p>
  </a>

  <a href="/FPMedio" class="plan">
    <h2>Grados Medios</h2>
    <p>Accede con el título de ESO, Bachillerato o mediante una prueba de acceso.</p>
  </a>
</div>


<div class="features-container">
  <div class="feature">
    <img src="/assets/images/aulamatinal_peq.png" class="feature-video">
    <div class="feature-content">
      <h2>Aula Matinal</h2>
      <p>JAPONEDUCA ofrece aula matinal en colegios, brindando a los alumnos un espacio seguro y enriquecedor para comenzar el día, facilitando además la organización de las familias.</p>
      <p style="text-align: center;"><button class="submit-button" onclick="location.href='https://japonformacion.netlify.app/aula_matinal/'">Saber más</button></p>
    </div>
  </div>

  <div class="feature">
    <div class="feature-content">
      <h2>Aula de Espera</h2>
      <p>JAPONEDUCA ofrece un servicio de aulas de espera en colegios, proporcionando un espacio seguro y supervisado para los alumnos, adaptándose a las necesidades familiares y escolares.</p>
      <p style="text-align: center;"><button class="submit-button" onclick="location.href='https://japonformacion.netlify.app/aula_espera/'">Saber más</button></p>
    </div>
    <video src="/assets/videos/Aula_de_Espera_2024-25.mp4" class="feature-video" autoplay loop muted></video>
  </div>

  <div class="feature">
    <img src="/assets/images/tatami_peq.png" class="feature-video">
    <div class="feature-content">
      <h2>Judo</h2>
      <p>Desde 1994, JAPONSPORT promueve el judo en Huelva para fomentar hábitos saludables y mejorar la calidad de vida.</p>
      <p style="text-align: center;"><button class="submit-button" onclick="location.href='https://japonformacion.netlify.app/judo/'">Saber más</button></p>
    </div>
  </div>

  <div class="feature">
    <div class="feature-content">
      <h2>FP Superior</h2>
      <p>Accede con el título de Bachillerato, una FP de Grado Medio o Superior o mediante prueba de acceso.</p>
      <p style="text-align: center;"><button class="submit-button" onclick="location.href='https://japonformacion.netlify.app/FPSuperior/'">Saber más</button></p>
    </div>
    <img src="/assets/images/CABECERA_peq.png" class="feature-video">
  </div>

  <div class="feature">
    <img src="/assets/images/CABECERA3_peq.png" class="feature-video">
    <div class="feature-content">
      <h2>FP Medio</h2>
      <p>Accede con el título de ESO, Bachillerato o mediante una prueba de acceso.</p>
      <p style="text-align: center;"><button class="submit-button" onclick="location.href='https://japonformacion.netlify.app/FPMedio/'">Saber más</button></p>
    </div>
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
  margin: 0;
  padding: 0.5em;
  color: inherit;
}

.video-container {
  margin: 0 auto;
  text-align: center;
}

.features-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

/* Default styling for larger screens */
.feature {
  display: flex;
  align-items: center;
  padding: 20px;
  margin-bottom: 40px;
}

.feature img {
  order: 0;
}

.feature:nth-child(even) img {
  order: 1;
}

/* Media query for smaller screens (e.g., below 768px) */
@media (max-width: 768px) {
  .feature {
    flex-direction: column;
  }
  
  /* Ensure images are always at the top on small screens */
  .feature img {
    order: -1 !important;
    width: 100%; /* Make images take full width on smaller screens if needed */
  }
  .feature video {
    order: -1 !important;
    width: 100%; /* Make images take full width on smaller screens if needed */
  }
}

.feature-content {
  display: flex;
  flex-direction: column;
  padding: 20px;
  text-align: center;
}

.feature-video {
  border-radius: 40px;
  width: 50%;
  height: auto;
  padding: 1em;
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
  color: black;
  outline: none;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-top: 1px solid #ccc;
}

.accordion-icon {
  transition: transform 0.3s ease;
}

.accordion-icon.rotated {
  transform: rotate(180deg);
}

.panel {
  padding: 0 18px;
  height: 0;
  overflow: hidden;
  transition: height 0.3s ease;
}

.panel.open {
  height: auto;
}

.plan-button {
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
