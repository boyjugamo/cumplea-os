<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mis XV Jimena Larissa</title>
<link rel="stylesheet" type="text/css" href="css/estilos.css">

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #F5A8ED;
  text-align: center;
}

nav {
  background: #e91e63;
  padding: 10px;
}
nav ul {
  list-style: none;
  padding: 0;
}
nav ul li {
  display: inline;
  margin: 10px;
}
nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

header {
  background: url("151.jpg") center/cover no-repeat;
  color: white;
  padding: 80px 20px;
}
header h1 {
  font-size: 40px;
}

section {
  background: white;
  margin: 20px;
  padding: 20px;
  border-radius: 10px;
}

.galeria img {
  width: 200px;
  margin: 10px;
  border-radius: 10px;
}

/* BOTON */
.boton {
  background: #e91e63;
  color: white;
  padding: 12px 20px;
  text-decoration: none;
  border-radius: 5px;
  display: inline-block;
  margin-top: 10px;
}

iframe {
  border-radius: 10px;
}

footer {
  background: #e91e63;
  color: white;
  padding: 10px;
}
</style>
</head>
<script>
const fechaEvento = new Date("Jul 18, 2026 20:00:00").getTime();

const contador = setInterval(function() {
  const ahora = new Date().getTime();
  const diferencia = fechaEvento - ahora;

  const dias = Math.floor(diferencia / (1000 * 60 * 60 * 24));
  const horas = Math.floor((diferencia % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  const minutos = Math.floor((diferencia % (1000 * 60 * 60)) / (1000 * 60));
  const segundos = Math.floor((diferencia % (1000 * 60)) / 1000);

  document.getElementById("tiempo").innerHTML =
    dias + " días " + horas + " horas " + minutos + " min " + segundos + " seg";

  if (diferencia < 0) {
    clearInterval(contador);
    document.getElementById("tiempo").innerHTML = "¡Hoy es el gran día!";
  }
}, 1000);
</script>

<body>

<!-- MENU -->
<nav>
  <ul>
    <li><a href="#inicio">Inicio</a></li>
    <li><a href="#evento">Evento</a></li>
    <li><a href="#galeria">Galería</a></li>
    <li><a href="#ubicacion">Ubicación</a></li>
    <li><a href="#confirmar">Confirmar</a></li>
  </ul>
</nav>

<!-- HEADER -->
<header id="inicio">
  <h1>Mis XV Jimena Larissa</h1>
  <p>¡Te invito a celebrar conmigo este día especial!</p>
</header>

<section id="contador">
  <h2>Faltan para mis XV</h2>
  <p id="tiempo"></p>
</section>

<!-- EVENTO -->
<section id="evento">
  <h2>Detalles del Evento</h2>
  <p><strong>Fiesta:</strong> 8:00 PM</p>
</section>

<section id="vestimenta">
  <h2>Código de Vestimenta</h2>
  <p>Queremos que todos disfruten este día especial 💖</p>
  
  <p><strong>Color reservado:</strong></p>
  <p style="color:#e91e63; font-weight:bold;">
    El color rosa está reservado exclusivamente para la quinceañera
  </p>

  <p>Te agradecemos evitar este color en tu vestimenta 🙏</p>
</section>

<!-- GALERIA -->
<section id="galeria" class="galeria">
  <h2>Galería</h2>
  <img src="imagen 2.jpg">
  <img src="imagen 3.jpg">
  <img src="images.jpg">
</section>

<!-- UBICACION -->
<section id="ubicacion">
  <h2>Ubicación</h2>
  <p>27294, M. Mercado de López Sánchez, 27294 Torreón, Coah.</p>

  <iframe 
    src="https://www.google.com/maps?q=27294,+M.+Mercado+de+L%C3%B3pez+S%C3%A1nchez,+Torre%C3%B3n,+Coahuila&output=embed"
    width="100%" 
    height="300" 
    loading="lazy">
  </iframe>

  <br><br>

  <a class="boton" 
     href="https://www.google.com/maps/place/SAL%C3%93N+%22QUINTA+LA+MARIA%22+%E2%9D%A4%EF%B8%8F%F0%9F%98%8E%F0%9F%98%98%F0%9F%91%8C/@25.5103734,-103.3810125,17.5z/data=!4m16!1m9!4m8!1m0!1m6!1m2!1s0x868fdd9b1c8d3df7:0x43578c93079c5d1e!2zU0FMw5NOICJRVUlOVEEgTEEgTUFSSUEiIOKdpO-4j_CfmI7wn5iY8J-RjCwgMjcyOTQsIE0uIE1lcmNhZG8gZGUgTMOzcGV6IFPDoW5jaGV6LCAyNzI5NCBUb3JyZcOzbiwgQ29haC4!2m2!1d-103.3782425!2d25.5103174!3m5!1s0x868fdd9b1c8d3df7:0x43578c93079c5d1e!8m2!3d25.5102486!4d-103.378232!16s%2Fg%2F11kprg5h6l?hl=es_419&entry=ttu&g_ep=EgoyMDI2MDQyMi4wIKXMDSoASAFQAw%3D%3D"
     target="_blank">
     Ver en Google Maps
  </a>
</section>

<!-- CONFIRMAR -->
<section id="confirmar">
  <h2>Confirmar Asistencia</h2>
  <p>Haz clic para confirmar por WhatsApp</p>

  <!-- CAMBIA EL NUMERO -->
  <a class="boton" 
     href="https://wa.me/528714662678?text=Hola%20confirmo%20mi%20asistencia%20a%20tus%20XV"
     target="_blank">
     Confirmar por WhatsApp
  </a>
</section>

<!-- FOOTER -->
<footer>
  <p>Con cariño, Ximena Larissa 💖</p>
</footer>

</body>
</html>
