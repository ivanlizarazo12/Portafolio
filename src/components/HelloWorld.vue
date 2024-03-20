<template>
  <div class="app" >
    <nav class="navbar navbar-expand-md bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">IVAN LIZARAZO</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <a class="nav-link active" aria-current="page" href="#">Sobre mi</a>
        <a class="nav-link" href="#">Experiencia</a>
        <a class="nav-link" href="#">Estudios</a>
        <a class="nav-link" href="#">Habilidades</a>
        <a class="nav-link" href="#">Mis proyectos</a>
        <a class="nav-link" href="#">Contactar</a>
      </div>
    </div>
  </div>
</nav>
 <!-- SOBRE MI -->
  
      <section id="about">
      <div class="container-card">
        <h2 >Sobre mi</h2>
        <div class="card"> 
          <div class="card-image-icons">
            <img src="../../public/Ivan1.jpg" class="card-img-top" alt="Photo">
            <div class="iconos">
              <i class="bi bi-github "></i>
              <i class="bi bi-linkedin "></i>
            </div>
          </div>
          <div class="card-content">
            <div class="card-body">
              <p class="card-text">Soy un tecnólogo en Análisis y Desarrollo de Sistemas de Información (ADSI) del SENA, con una pasión por el aprendizaje autodidacta y una habilidad innata para adquirir rápidamente nuevos conocimientos. Me distingo por mi disposición para ayudar y mi capacidad para trabajar en equipo.</p>
              <p class="card-text">Enfocándome en el crecimiento personal y profesional, mis objetivos a corto plazo incluyen el aprendizaje del inglés y la mejora continua de mis habilidades de desarrollo de software. Estoy convencido de que el éxito en el desarrollo de software no solo depende de las habilidades técnicas, sino también de la capacidad para colaborar y comunicarse eficazmente con los demás.</p>
              <p class="card-text">A largo plazo, aspiro a convertirme en un desarrollador de software altamente competente, capaz de aportar valor a cualquier equipo o proyecto en el que participe. Estoy emocionado por las oportunidades que me esperan en el campo de la tecnología y estoy listo para enfrentar los desafíos que vengan.</p>
            </div>
          </div>
        </div>
      </div>  
    </section>

    <section id="experience">
      <h2>Experiencia</h2>
      <div class="experience-card">
        <h4>Tecnoparque nodo Socorro</h4>
        <p>Apoyo a la linea de tecnologias virtuales</p>
        <p>01/11/2023 - Presente</p>
        <p>Durante mis prácticas en Tecnoparque, he trabajado en el desarrollo de aplicaciones web utilizando Vue.js 3 y Firebase. Esta experiencia me ha permitido aplicar mis habilidades técnicas y entender la importancia de crear soluciones que aporten valor a los negocios.</p>
        <p><strong>Habilidades adquiridas:</strong></p>
        <ul>
          <li>Desarrollo frontend con Vue.js 3</li>
          <li>Uso de Firebase para el backend</li>
          <li>Trabajo en equipo en un entorno de desarrollo ágil</li>
          <li>Manejo de herramientas ofimaticas</li>
          <li></li>
        </ul>
      </div>
    </section>

    <section>
      <section>
  <h2> Habilidades</h2>
  <div class="experience-card">
    <div class="container-logos"></div>
    <div class="row">
      <div class="col-lg-4" v-for="(logo, index) in logos" :key="index">
        <div class="card mb-3 logo-card">
          <div class="card-body">
            <img :src="`/logos/${logo}`" class="logo-img">
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
</section>

    <section>
      <div class="row">
        <div class="col-lg-6">
          <h2>Estudios</h2>
          <div class="card mb-3" style="background-color: #2a2f4a;">
            <div class="card-body">
              <h5 class="card-title">Analista y Desarrollo de Sistemas de Información - SENA</h5>
              <p class="card-text">Actualmente cursando este programa de formación en el SENA. He adquirido habilidades en...</p>
            </div>
          </div>
        </div>

        <div class="col-lg-6">
          <h2>Mis proyectos</h2>
          <div class="card mb-3" style="background-color: #2a2f4a;">
            <div class="card-body">
              <h5 class="card-title">Analista y Desarrollo de Sistemas de Información - SENA</h5>
              <p class="card-text">Actualmente cursando este programa de formación en el SENA. He adquirido habilidades en...</p>
            </div>
          </div>
        </div>
      </div>

    </section>
    <div class="contact-section" style="background-color: #1c2030; color: #e5e5e5;">
    <div class="container">
      <h2 class="section-title">Contáctame</h2>
      <div class="row justify-content-center">
        <div class="col-auto">
          <a href="mailto:tu_correo@ejemplo.com" target="_blank">
            <i class="fas fa-envelope fa-2x"></i>
            <p>Correo</p>
          </a>
        </div>
        <div class="col-auto">
          <a href="https://www.linkedin.com/in/tu_usuario/" target="_blank">
            <i class="fab fa-linkedin fa-2x"></i>
            <p>LinkedIn</p>
          </a>
        </div>
        <div class="col-auto">
          <a href="https://github.com/tu_usuario" target="_blank">
            <i class="fab fa-github fa-2x"></i>
            <p>GitHub</p>
          </a>
        </div>
        <div class="col-auto">
          <a href="https://wa.me/tu_numero" target="_blank">
            <i class="fab fa-whatsapp fa-2x"></i>
            <p>WhatsApp</p>
          </a>
        </div>
      </div>
  </div>
  </div>
</div>

</template>

<script setup>

import { ref } from 'vue';

const logos = ref([
  'Boostrap.png',
  'css.png',
  'Firebase.png',
  'html.png',
  'JavaScript.png',
  'node.png',
  'Vue.png',
]);
</script>

<style scoped>

.logo-card {
  height: 100px; /* Ajusta esto al tamaño que prefieras */

}

.logo-img {
  max-width: 100%;
  max-height: 100%;
  object-fit: cover;
  border-radius: 0;
}

.app {
  background-color: #1c2030;
}
.navbar {
  padding: 10px;
  
  background-color:#c5d6e8;
}
.nav-link{
  border-radius:7px;
  border: #1c2030;
  padding:  3px;
  margin: 0px 1px 0px 1px;
  background-color: #e5e5e5;
  color: #1c2030;
  text-decoration: none;
  border-bottom: none;
}
.card {
  padding: 10px;
  background-color: #1c2030;
  width: 95%;
  display: flex;
  flex-direction: row;
}
.container-card {
  margin: 10px;
  min-width: 100%;
}
.card-image-icons {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-right: 10px;
}
.card-content {
  flex-grow: 1;
}
.card-img-top {
  margin-top: 35px;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.iconos {
  padding: 5px;
  display: flex;
  justify-content: center;
  flex-direction: row;
  color: #f3f3f3;
}


.iconos i {
  margin: 0 5px; 
}
.card-text {
  color: #f3f3f3;
  font-size: small;
}
h2{
  color: #f3f3f3;
  text-align: center;
}
h4 {
  color: #e5e5e5;
}
p {
  color: #f3f3f3;
}


.experience-card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  border-radius: 5px; /* 5px rounded corners */
  border: 1px solid #ddd; /* Border color */
  margin: 20px; /* Space around the card */
  padding: 20px; /* Space around the content */
  background-color: #1c2030; /* Background color */
  color: #f3f3f3; /* Text color */
}

/* On mouse-over, add a deeper shadow */
.experience-card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

/* Estilos para el título de la tarjeta */
.experience-card h4 {
  color: #e5e5e5;
  font-size: 1.25rem;
  font-weight: bold;
}

/* Estilos para el texto de la tarjeta */
.experience-card p {
  color: #f3f3f3;
  font-size: 1rem;
  line-height: 1.5;
}


.contact-section {
  padding: 60px 0;
}

.section-title {
  text-align: center;
  margin-bottom: 50px;
  font-size: 2.5em;
}

a {
  color: #e5e5e5;
  text-decoration: none;
  text-align: center;
  display: block;
}

a:hover {
  color: #e5e5e5;
}

i {
  margin-bottom: 10px;
}
</style>