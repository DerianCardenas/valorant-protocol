<template>
  <div class="home" id="home">
    <img alt="Valorant" className="img-valorant m-5" src="@/assets/valoran-logo.png">
    <div className="parallax"><br/>
      <p className="p-princ">
        Valorant es un hero shooter en primera persona multijugador gratuito desarrollado y publicado por Riot Games. El juego se anunció por primera vez con el nombre en clave Project A en octubre de 2019. Fue lanzado para Microsoft Windows el 2 de junio de 2020 después de su beta cerrada lanzada el 7 de abril de 2020.
      </p>
      <h2>JUEGA A TU MANERA</h2>
        <p>
          Combina tu estilo y experiencia en un escenario global y competitivo. Tienes 13 rondas para atacar y defender tu lado con armas precisas y habilidades tácticas. Además, al contar con una sola vida por ronda, tendrás que pensar más rápido que tu oponente si quieres sobrevivir. Enfréntate a enemigos en los modos competitivo y normal, así como en Deathmatch y Spike Rush.
        </p>
        </div>
      <h2 className="mid-h2">ESCOGE ENTRE 19 AGENTES</h2>
      <div className="parallax par-2"><br/>
        <p className="p-princ">
          Más allá de las armas y las balas, podrás elegir a un agente dotado de habilidades versátiles, veloces y letales con las que crearás oportunidades para sobresalir. Ningún agente se jugará igual, ni ningún momento memorable se verá igual.
        </p>
      <h2>COMBATE ALREDEDOR DEL MUNDO</h2>
        <p>Cada mapa es un campo de batalla para demostrar tu pensamiento creativo. Están diseñados especialmente para estrategias de equipo, jugadas espectaculares y momentos para remontar. Haz la jugada que otros imitarán en el futuro.
        </p>
        <a className="subir" href="#home">Ir Arriba</a>
        <br/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
export default {
  name: 'HomeView'
}
</script>
<style scoped>
  .img-valorant{
    max-width:720px;
  }
  h2{
    color:white;
    margin: 0 auto;
    width: 20%;
  }
  .mid-h2{
    color:crimson;
    height: 50px;
    margin:2em auto;
  }
  .parallax{
    background-image: url('../assets/img1.jpeg');

    height: 700px; 

    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  .par-2{
    background-image: url('../assets/img2.jpeg');
    margin-top:3em;
  }
  .p-princ{
    margin-top: 3em;
  }
  p{
    background: #ff3232;
    /* Old browsers */
    background: linear-gradient(to right, white 50%, crimson 50%);
    background-size: 200% 100%;
    background-position:left bottom;
    border-radius:1.5em;
    display:flex;
    margin: 3em auto;
    padding:2em;
    text-align:center;
    transition:all 1s ease;
    width:80%;
  }
  p:hover{   
    background-position:right bottom;
    color:white;
  }
  .subir{
    border-top-right-radius: 5em;
    border-bottom-left-radius: 5em;
    background-color: crimson;
    color:white;
    margin:3em auto;
    padding:1em 3em;
    text-decoration:none;
  }
</style>
