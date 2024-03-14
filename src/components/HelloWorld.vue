<template>
  <div class="app" >
    <nav class="navbar navbar-expand-lg">
      <a class="navbar-brand" >Ivan Lizarazo</a>
      <div class="navbar-collapse" id="navbarNav">
        <button class="nav-link" href="#about"> Acerca de mi</button>
        
        <button class="nav-link" href="#projects"> Acerca de mi</button>
        <button class="nav-link" href="#contact"> Acerca de mi</button>
      </div>
    </nav>
    <section id="about">
      <h2>Acerca de mi </h2>

      <img class="foto" src="../../public/Ivan1.jpg" alt="Photo">
      <div class="iconos">
      <i class="bi bi-github"></i>
      <i class="bi bi-linkedin"></i>
      </div>
      <p>Ifo</p>
    </section>
    <section>
      
      <h2 >Experiencia</h2>
      <p>Info</p>
    </section>
    <section>
      <h2>Estudios</h2>
      <p>info</p>
    </section>
    <section>
      <h2> Habilidades</h2>
      <p>info</p>
    </section>
    <section id="projects">
      <h2>Mis proyectos</h2>
      <p>Ifo</p>
    </section>
    <section id="contact">
      <h2>Contacto</h2>
      <p>Ifo</p>
    </section>
  </div>
</template>

<script>

</script>

<style scoped>
.navbar {
  padding: 10px;
  
  background-color:#c5d6e8;
  display: flex;
  justify-content: space-between;
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

.app {
  background-color: #1c2030;
}

.foto {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.iconos {
  text-align: center;
  color: #f3f3f3;
}


h2{
  color: #f3f3f3;
  text-align: center;

}
p {
  color: #f3f3f3;
}
</style>