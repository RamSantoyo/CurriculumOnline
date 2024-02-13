<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { ref, computed } from 'vue'
import { storeToRefs } from 'pinia';
import cabecera from './views/titular.vue'
import info from './views/info.vue'
import estudios from './views/estudios.vue'
import cursos from './views/cursos.vue'
import experence from './views/experiencia.vue'
import portafolio from './views/portafolio.vue'
import skills from './views/skills.vue'

const modo = ref(false);
let body = document.querySelector('body');

const cambiar = () => {
  if (modo.value == false) {
    modo.value = true;
    body.classList.add('dark');
  } else {
    modo.value = false;
    body.classList.remove('dark');
  }
}

</script>

<template>
  <div>
    <div class="contenedor">
      <header>
        <div class="logo">
          <h1 class="p1">Ramsess</h1>
          <h1 class="p2">Santoyo</h1>
        </div>
        <nav>
          <a href="https://github.com/RamSantoyo" target="_blank"><i class="fa-brands fa-github"></i></a>
          <a href="https://www.instagram.com/ramsantoyo/" target="_blank"><i class="fa-brands fa-instagram"></i></a>
          <a href="https://www.tiktok.com/@jrdeveloper?_t=8XOH9F9fqT8&_r=1" target="_blank">
            <i class="fa-brands fa-tiktok"></i></a>
          <a href="https://api.whatsapp.com/send/?phone=525531567430&text=Hola+Ramsess&app_absent=0" target="_blank">
            <i class="fa-brands fa-whatsapp"></i></a>
          <label class="switch">
            <input type="checkbox" @click="cambiar">
            <span class="slider"></span>
          </label>
        </nav>
      </header>
      <cabecera />
      <info />
      <estudios />
    </div>
    <section class="cursos">
      <div class="contenedor">
        <cursos />
      </div>
    </section>
    <div class="contenedor">
      <experence />
      <portafolio />
      <skills />
    </div>
    <footer>
      <div class="contenedor footer">
        <div class="logo">
          <h1 class="p1">Ramsess</h1>
          <h1 class="p2">Santoyo</h1>
        </div>
        <div class="fot-2">
          <nav class="iconos-blc">
            <a href="https://github.com/RamSantoyo" target="_blank">
              <i class="fa-brands fa-github"></i>
            </a>
            <a href="https://www.instagram.com/ramsantoyo/" target="_blank">
              <i class="fa-brands fa-instagram"></i>
            </a>
            <a href="https://www.tiktok.com/@jrdeveloper?_t=8XOH9F9fqT8&_r=1" target="_blank">
              <i class="fa-brands fa-tiktok"></i>
            </a>
            <a href="https://api.whatsapp.com/send/?phone=525531567430&text=Hola+Ramsess&app_absent=0" target="_blank">
              <i class="fa-brands fa-whatsapp"></i>
            </a>
          </nav>
          <p class="copy">All rights reserved &copy; 2023</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<style scoped>
.logo {
  display: flex;
  font-family: var(--fuente-1);
  font-size: 1.3rem;
}

.p1 {
  font-weight: var(--regular500);
  color: var(--colorprimario);
}

.p2 {
  font-weight: var(--delgada200);
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 3rem;
}

.fa-brands {
  font-size: 1.8rem;
  color: var(--colorterceario);
}

.fa-brands:hover {
  color: var(--colorprimario);
}

/*Boton*/
/* The switch - the box around the slider */
.switch {
  font-size: 17px;
  position: relative;
  display: inline-block;
  width: 3.5em;
  height: 2em;
}

/* Hide default HTML checkbox */
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

/* The slider */
.slider {
  --background: #28096b;
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: var(--background);
  transition: .5s;
  border-radius: 30px;
}

.slider:before {
  position: absolute;
  content: "";
  height: 1.4em;
  width: 1.4em;
  border-radius: 50%;
  left: 10%;
  bottom: 15%;
  box-shadow: inset 8px -4px 0px 0px #fff000;
  background: var(--background);
  transition: .5s;
}

input:checked+.slider {
  background-color: var(--colorterceario);
}

input:checked+.slider:before {
  transform: translateX(100%);
  box-shadow: inset 15px -4px 0px 15px #fff000;
}

.cursos {
  background-color: var(--colorsecundario);
  margin-top: 4rem;
  padding-top: 2rem;
  margin-bottom: 4rem;
  padding-bottom: 8rem;
}

footer {
  background-color: var(--colorprimario);
  color: white;
}

.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem;
  margin-top: 4rem;
}

.footer .logo .p1 {
  color: var(--colorterceario);
}

.copy {
  font-size: 1.2rem;
  font-weight: var(--regular500);
  text-align: right;
}

.fot-2 {
  display: flex;
  flex-direction: column;

}

.iconos-blc a i {
  color: white;
}

.iconos-blc a i:hover {
  color: var(--colorsecundario);
}

@media (max-width: 575px) {
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2rem;
  }

  .footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;
  }
}
</style>
