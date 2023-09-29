<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'

</script>

<template>
  <header class="full-header w-full">
    <div class="overlayd">
      <div class="titles">
        <img src="./assets/ziklag.png">
        <div class="language-switcher">
            <span>
              <img src="./assets/en.png">  
              English
            </span> 
            <span>
              <img src="./assets/es.png">  
              Espanol
            </span>
            <span>
              <img src="./assets/pt.png">  
              Portugues
            </span>
            <span>
              <img src="./assets/em.png">  
              Arabe
            </span>
        </div>
      </div>
      <nav class="first-nav">
        <RouterLink to="/">Inicio</RouterLink>
        <a href="#services">Servicios</a>
        <RouterLink to="/about">Productos</RouterLink>
        <RouterLink to="/about">Solicitar Cotizacion</RouterLink>
        <a href="#us">Nosotros</a>
        <RouterLink to="/about">Contactame</RouterLink>
      </nav>
      <nav class="responsive-nav">
        <div class="">
          <span class="toggler">
            <img src="./assets/menu.png">
          </span>
        </div>
        <ul>
          <li>
            <RouterLink to="/">Inicio</RouterLink>
          </li>
          <li>
            <RouterLink to="/about">Servicios</RouterLink>
          </li>
          <li>
            <RouterLink to="/about">Productos</RouterLink>
          </li>
          <li>
            <RouterLink to="/about">Solicitar Cotizacion</RouterLink>
          </li>
          <li>
            <RouterLink to="/about">Idea de Flete</RouterLink>
          </li>
        </ul>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

</style>
