---
title: "Judo"
permalink: /judo/
layout: default
---



<div class="splash-container">
  <!-- Full-width background image -->
  <img src="/assets/images/tatami.png" alt="Full Width Image" class="splash-image">

  <!-- Grey transparent background image -->
  <div class="grey-background"></div>

  <!-- Text title at top right -->
  <div class="top-left">Judo</div>

  <!-- Right image upfront -->
  <img src="/assets/images/judoka.png" alt="Right Image" class="right-image">

  <!-- Text content at bottom left -->
  <div class="bottom-left">
    <p>JAPONSPORT, C.D., fundada en 1994 como parte del GRUPO JAPÓN, ofrece actividades extraescolares en Huelva y su provincia. Se enfoca en crear escuelas deportivas y promover hábitos saludables con personal cualificado. Evolucionó del Club "Juji-Japón", la primera escuela de judo en Huelva, fundada por el maestro José González Japón, y ofrece dos niveles de judo según la edad y el nivel de cinturón.</p>
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
    width: 360px;
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
    margin-right: 13em;
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
</style>


<div style="font-size: 17px;text-align: center;">
  <p>Fecha de inicio: 1 de octubre de 2024</p>
</div>


<div class="table-container">
<table>
  <thead>
    <tr>
      <th style="width: 200px;text-align: center;"><h2>Escuela</h2></th>
      <th style="width: 200px;text-align: center;"><h2>Actividad</h2></th>
      <th style="width: 200px;text-align: center;"><h2>Edad</h2></th>
      <th style="width: 200px;text-align: center;"><h2>Horario</h2></th>
      <th style="width: 200px;text-align: center;"><h2>Cuota</h2></th>
      <th style="width: 200px;text-align: center;"><h2>Enlaces</h2></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="width: 200px;text-align: center; vertical-align: middle;" rowspan="2">Grupo Japón</td>
      <td style="width: 200px;text-align: center;">Judo 1</td>
      <td style="width: 200px;text-align: center;">De 4 a 8 años</td>
      <td style="width: 200px;text-align: center;">Lunes y miércoles de 18:00 a 19:00 h</td>
      <td style="width: 200px;text-align: center;"> 25 €/mes* </td>
      <td style="width: 200px;text-align: center;">
        <ul style="list-style-type: disc; padding-left: 40px; margin: 0; text-align: left;">
          <li><a href="/assets/documents/CUOTAS_Y_FORMAS_DE_PAGO_JAPONSPORT_HUELVA_2024-25.pdf">Forma de pago</a></li>
          <li><a href="/assets/documents/HORARIO_GRUPO_JAPON_JUDO_JAPONSPORT_2024-25_XaUUYYm.pdf">Horario</a></li>
          <li><a href="https://app.grupojapon.es/index.php/registro">Inscríbete</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="width: 200px;text-align: center;">Judo 2</td>
      <td style="width: 200px;text-align: center;">De 9 a 15 años</td>
      <td style="width: 200px;text-align: center;">Lunes y miércoles de 19:00 a 20:00 h</td>
      <td style="width: 200px;text-align: center;"> 30 €/mes* </td>
      <td style="width: 200px;text-align: center;">
        <ul style="list-style-type: disc; padding-left: 40px; margin: 0; text-align: left;">
          <li><a href="/assets/documents/CUOTAS_Y_FORMAS_DE_PAGO_JAPONSPORT_HUELVA_2024-25.pdf">Forma de pago</a></li>
          <li><a href="/assets/documents/HORARIO_GRUPO_JAPON_JUDO_JAPONSPORT_2024-25_XaUUYYm.pdf">Horario</a></li>
          <li><a href="https://app.grupojapon.es/index.php/registro">Inscríbete</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="width: 200px;text-align: center; vertical-align: middle;" rowspan="2">CEIP El Puntal</td>
      <td style="width: 200px;text-align: center;">Judo 1</td>
      <td style="width: 200px;text-align: center;">De 4 a 8 años</td>
      <td style="width: 200px;text-align: center;">Martes y jueves de 18:00 a 19:00 h</td>
      <td style="width: 200px;text-align: center;"> 25 €/mes* </td>
      <td style="width: 200px;text-align: center;">
        <ul style="list-style-type: disc; padding-left: 40px; margin: 0; text-align: left;">
          <li><a href="/assets/documents/CUOTAS_Y_FORMAS_DE_PAGO_JAPONSPORT_BELLAVISTA_2024-25.pdf">Forma de pago</a></li>
          <li><a href="/assets/documents/HORARIO_CEIP_EL_PUNTAL_JUDO_JAPONSPORT_2024-25_RcKb3CC.pdf">Horario</a></li>
          <li><a href="https://app.grupojapon.es/index.php/registro">Inscríbete</a></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td style="width: 200px;text-align: center;">Judo 2</td>
      <td style="width: 200px;text-align: center;">De 11 a 15 años</td>
      <td style="width: 200px;text-align: center;">Martes y jueves de 19:00 a 20:00 h</td>
      <td style="width: 200px;text-align: center;"> 30 €/mes* </td>
      <td style="width: 200px;text-align: center;">
        <ul style="list-style-type: disc; padding-left: 40px; margin: 0; text-align: left;">
          <li><a href="/assets/documents/CUOTAS_Y_FORMAS_DE_PAGO_JAPONSPORT_BELLAVISTA_2024-25.pdf">Forma de pago</a></li>
          <li><a href="/assets/documents/HORARIO_CEIP_EL_PUNTAL_JUDO_JAPONSPORT_2024-25_RcKb3CC.pdf">Horario</a></li>
          <li><a href="https://app.grupojapon.es/index.php/registro">Inscríbete</a></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


</div>

<div style="font-size: 17px;text-align: center;font-style: italic;">
  <p style="margin-bottom: 6em;">*Bonificación del 10% para el segundo o tercer hermano inscrito</p>
</div>



<div style="text-align:center; margin: 2em;">
  Documentos útiles para usuarios
</div>

<p style="
    text-align: center;
"><a href="/assets/documents/NOTA INFORMATIVA LICENCIA Y C GRADO JUDO 24-25.pdf" rel="nofollow noopener noreferrer" style="font-size: 17px;">Cómo tramitar licencias</a>
<a href="/assets/documents/Categorias y pesos Fanjyda 2024-25.png" rel="nofollow noopener noreferrer" style="font-size: 17px;">Categorias y pesos Fanjyda 2024-25</a>
</p>


<div style="text-align:center; margin: 2em; margin-top: 4em;">
  Preguntas frecuentes
</div>

<div class="faq-container">
  <div id="faq" class="faq">
    <button class="accordion">¿Cuándo se abre el periodo de inscripción?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>A partir del 1 de septiembre de 2024.</p>
    </div>

    <button class="accordion">¿Cuándo empiezan y terminan las clases?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>Desde el 1 de octubre de 20024 al 30 de mayo de 2025.</p>
    </div>

    <button class="accordion">¿Dónde puedo conseguir mi kimono?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>En tiendas de deportes o en nuestras oficinas en C/Santiago Apóstol nº 37 Huelva (horario de mañana).</p>
    </div>

    <button class="accordion">¿Hay descuentos en las cuotas?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>Sí. 10% de descuento a partir del 2º hermano/a.</p>
    </div>

    <button class="accordion">¿Cuál es la forma de pago y cuándo pasan los recibos al cobro?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>Se realizará por anticipado del 1 al 5, trimestralmente, a través de Domiciliación Bancaria (octubre, noviembre y diciembre se cobrarán juntos en noviembre). Los siguientes trimestres se cobraran en febrero y en mayo.</p>
    </div>

    <button class="accordion">¿Cómo me doy de baja?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>Enviado un email a través de nuestro correo: contacto@grupojapon.es.</p>
    </div>

    <button class="accordion">Si me doy de baja antes del término del trimestre abonado, ¿me devuelven los meses no asistido?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>Sí. Se realizara la devolución a través de transferencia de los meses no asistidos.</p>
    </div>

    <button class="accordion">Si quiero participar en Campeonatos, ¿Qué debo hacer?
      <img src="/assets/images/angulo-hacia-abajo.png" width="20" height="20" class="accordion-icon">
    </button>
    <div class="panel">
      <p>Estar dados de alta en la federación. Información a través del siguiente enlace: PINCHE AQUÍ este es el enlace: (https://www.grupojapon.es/media/documentos/1/NOTA_INFORMATIVA_LICENCIA_Y_C_GRADO_JUDO_23-24_Ap7M8rR.pdf)</p>
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
  background-color: #e31c24;
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
