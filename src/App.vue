<template>
  <nav>
    <router-link to="/">Inicio</router-link>
    <router-link to="/agentes">Agentes</router-link>
    <router-link to="/mapas">Mapas</router-link>
    <router-link to="/armas">Armas</router-link>
    <router-link to="/valorant">Valorant</router-link>
  </nav>
  <router-view/>
</template>

<style>
  @import url('http://fonts.cdnfonts.com/css/valorant');
*{
  font-family: 'VALORANT', sans-serif;
  margin:0;
  padding:0;
     scroll-behavior: smooth;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  animation: fadeInAnimation ease 1.5s;
  animation-iteration-count: 1;
  animation-fill-mode: forwards;
}
  
@keyframes fadeInAnimation {
    0% {
        opacity: 0;
    }
    100% {
        opacity: 1;
     }
}
nav {
  background-color: crimson;
  padding: 1.5em;
}

nav a {
  border-radius: 1em;
  color: white;
  font-size:1.2em;
  margin: auto 1.5em;
  text-align: center;
  text-decoration: none;
  padding:.75em 2em;
  transition:all 1s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}
nav a:hover{
  background-color: white;
  color: crimson;
  text-decoration: none;;
}
nav a.router-link-exact-active {
  background-color: white;
  color: crimson;
}
</style>
