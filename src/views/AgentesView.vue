<template>
  <div className="container-princ">
    <img alt="Valorant" className="img-valorant m-5" src="@/assets/valoran-logo.png">
    <p className="agentes-view">
      Los agentes son los personajes jugables que representan a cada miembro del protocolo Valorant.
      Cada agente tiene su propia clase y cuenta con 4 habilidades diferentes que te ayudarán a completar la misión.
      La mayoría de los agentes se desbloquean cumpliendo su contrato, consiguiendo recompensas en el camino.
    </p>
    <h2>LISTADO DE AGENTES</h2>
    <div className="cont-agents parallax" id="contenedor">
      <div className="list-agents">
        <button @click="mostrar(1)">01 - Brimstone</button><br/>
        <button @click="mostrar(2)">02 - Viper</button><br/>
        <button @click="mostrar(3)">03 - Omen</button><br/>
        <button @click="mostrar(4)">04 - Killjoy</button><br/>
        <button @click="mostrar(5)">05 - Cypher</button><br/>
        <button @click="mostrar(6)">06 - Sova</button><br/>
        <button @click="mostrar(7)">07 - Sage</button><br/>
        <button @click="mostrar(9)">09 - Phoenix</button><br/>
        <button @click="mostrar(10)">10 - Jett</button><br/>
        <button @click="mostrar(11)">11 - Reyna</button><br/>
        <button @click="mostrar(12)">12 - Raze</button><br/>
        <button @click="mostrar(13)">13 - Breach</button><br/>
        <button @click="mostrar(14)">14 - Skye</button><br/>
        <button @click="mostrar(15)">15 - Yoru</button><br/>
        <button @click="mostrar(16)">16 - Astra</button><br/>
        <button @click="mostrar(17)">17 - KAY/O</button><br/>
        <button @click="mostrar(18)">18 - Chamber</button><br/>
        <button @click="mostrar(19)">19 - Neon</button><br/>
        <button @click="mostrar(20)">20 - Fade</button><br/>
      </div>
      <div className="desc-agents" id="show">
        <div className="list-agent-info" id="agent-info">
            <div className="info-basica">
              <li>Nombre: {{agentes[index].nombre}}</li>
              <li>Nombre Real: {{agentes[index].real}}</li>
              <li>Rol: {{agentes[index].rol}}</li>
              <li>Pais:{{agentes[index].pais}}</li>
              <li>Habilidad 1: {{agentes[index].basica1}}</li>
              <li>Habilidad 2: {{agentes[index].basica2}}</li>
              <li>Habilidad Clave: {{agentes[index].especial}}</li>
              <li>Habilidad Definitiva: {{agentes[index].definitiva}}</li>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
/* eslint-disable */
  export default {
    name:'AgentesView',
    scrollPosition:null,
    data(){
      return{
        agentes:[{},
        {
              "nombre":"Brimstone",
              "real":"Liam Byrne",
              "pais":"Estados Unidos",
              "rol":"Controlador",
              "basica1":"Incendiaria",
              "basica2":"Baliza Potenciadora",
              "especial":"Humo Celestial",
              "definitiva":"Ataque Orbital"
        },{
              "nombre":"Viper",
              "real":"Sabine Callas",
              "pais":"Estados Unidos",
              "rol":"Controlador",
              "basica1":"Mordedura",
              "basica2":"Nube Venenosa",
              "especial":"Cortina Toxica",
              "definitiva":"Pozo de la Vibora"
        },{
              "nombre":"Omen",
              "real":"John/Fred/Marcus/Yohan/Dimitri",
              "pais":"Desconocido / Planeta Tierra",
              "rol":"Controlador",
              "basica1":"Paso Sombrio",
              "basica2":"Paranoia",
              "especial":"Manto Oscuro",
              "definitiva":"Desde las sombras"
        },{
              "nombre":"Killjoy",
              "real":"Klara Böhringer",
              "pais":"Alemania",
              "rol":"Controlador",
              "basica1":"Bot de Alarma",
              "basica2":"NanoEnjambre",
              "especial":"Torreta",
              "definitiva":"Dispositivo Inmovilizador"
        },{
              "nombre":"Cypher",
              "real":"Amir El Amari",
              "pais":"Marruecos",
              "rol":"Centinela",
              "basica1":"Ciberjaula",
              "basica2":"Cable Trampa",
              "especial":"Cámara Espía",
              "definitiva":"Asalto Neural"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron Búho",
              "especial":"Dardo de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sage",
              "real":"Ling Ying Wei",
              "pais":"China",
              "rol":"Centinela",
              "basica1":"Orbe Ralentizador",
              "basica2":"Orbe de Barrera",
              "especial":"Orbe Curativo",
              "definitiva":"Resurrección"
        },{},{
              "nombre":"Phoenix",
              "real":"Jamie Adeyemi",
              "pais":"Reino Unido",
              "rol":"Duelista",
              "basica1":"Destello en Curva",
              "basica2":"Muro Abrasador",
              "especial":"Manos Calientes",
              "definitiva":"Va de Fuego"
        },{
              "nombre":"Jett",
              "real":"Sunwoo Han",
              "pais":"Corea del Sur",
              "rol":"Duelista",
              "basica1":"Ráfaga Ascendente",
              "basica2":"Nube Explosiva",
              "especial":"Impulso Ciclón",
              "definitiva":"Tormenta de Cuchillas"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        },{
              "nombre":"Sova",
              "real":"Alexander (Sasha) Novikov",
              "pais":"Rusia",
              "rol":"Iniciador",
              "basica1":"Dardo Electrico",
              "basica2":"Dron de Reconocimiento",
              "especial":"Flecha de Rastreo",
              "definitiva":"Furia del Cazador"
        }],
        index:0
      }
    },
    methods:{
      mostrar(num){
        this.index=num;
        let contenedor = document.getElementById("contenedor");
        contenedor.className=`parallax wall-${num}`
        let info = document.getElementById("agent-info");
        if(this.index!=0)
          info.classList="reveal";
      }
    }
  }
</script>
<style scoped>
.img-valorant{
    max-width:720px;
  }
  .container-princ{
    padding-top:2em ;
  }
  .agentes-view{
    display:flex;
    margin: 2em auto;
    font-size:1.5em;
    text-align:justify;
    width:80%;
  }
  h2{
    background-color: white;;
    /*background-image: linear-gradient(white,crimson); */
    margin:0;
    padding-top:3em;
    padding-bottom:3em;
  }
  .parallax{
    /* Create the parallax scrolling effect */
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    display:flex;
    height:max-content;
    width: 100%;
  }
  .cont-agents{
    background-image: url('../assets/poster-agentes.jpg');
}
  .wall-1{background-image: url('../assets/personajes/Brimstone/fondo.jpeg');}
  .wall-2{background-image: url('../assets/personajes/Viper/fondo.jpg');}
  .wall-3{background-image: url('../assets/personajes/Omen/fondo.jpg')}
  .wall-4{background-image: url('../assets/personajes/Killjoy/fondo.jpg')}
  .wall-5{background-image: url('../assets/personajes/Cypher/fondo.jpeg')}
  .wall-6{background-image: url('../assets/personajes/Sova/fondo.jpg');}
  .wall-7{background-image: url('../assets/personajes/Sage/fondo.jpeg');}
  .wall-9{background-image: url('../assets/personajes/Phoenix/fondo.jpg'); }
  .wall-10{background-image: url('../assets/personajes/Jett/fondo.jpg'); }
  .list-agents{
    display:block;
    width: 40%;
  }
  .desc-agents{
    color:white;
    margin:0;
    position: relative;
    width:60%;
  }
  .list-agent-info{
    display:none;
  }
  .reveal{
    background-color:rgba(220, 20, 60, 0.705);
    top: 50px;
    display:block;
    list-style: none;
    margin: 5em 0;
    position:sticky;
  }
  li{
    font-family:Arial, Helvetica, sans-serif;
    font-weight: bolder;
  }
  .info-basica{
    font-size:1.5em;
    padding: 5em;
  }
  button{
    border:none;
    background-color: transparent;
    color:black;
    margin-top: 2em;
    font-family:Arial, Helvetica, sans-serif;
    font-size:50px;
    font-weight: bolder;
    text-align:left;
    text-shadow: 0 0 5px white;
    transition: all .85s cubic-bezier(0.455, 0.03, 0.515, 0.955);
    width:70%;
  }
  button:hover{
    color:white;
    cursor:pointer;
    text-shadow: 0 0 7px crimson;
    transform:translateX(15%);
  }
</style>
