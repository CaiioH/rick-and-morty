<template>
  <div class="container"> <!--Container da pagina toda-->
    <div class="containercard">
      <div class="allcards">
        <!-- Morty -->
        <div class="card">
          <img src="../assets/Personagens/morty.jpeg" alt="Imagem do card" />
          <h2>Titulo Grande pra caralho Titulo Grande pra caralho</h2>
          <div id="paragrafos">
            <p id="p1">Last known location: {{ localizacao }}</p>
            <p id="p2">First seen in: {{ primeiroVisto }}</p>
          </div>
        </div>

        <!-- Baby Rick -->
        <div class="card">
          <img src="../assets/Personagens/BabyRick.jpeg" alt="Imagem do card" />
          <h2>{{ titulo }}</h2>
          <div id="paragrafos">
            <p id="p1">Last known location: {{ localizacao }}</p>
            <p id="p2">First seen in: {{ primeiroVisto }}</p>
          </div>
        </div>

        <!-- Roy's Son  -->
        <div class="card">
          <img src="../assets/Personagens/RoySon.jpeg" alt="Imagem do card" />
          <h2>{{ titulo }}</h2>
          <div id="paragrafos">
            <p id="p1">Last known location: {{ localizacao }}</p>
            <p id="p2">First seen in: {{ primeiroVisto }}</p>
          </div>
        </div>

        <!-- Mechanical Rick  -->
        <div class="card">
          <img src="../assets/Personagens/MechanicalRick.jpeg" alt="Imagem do card" />
          <h2>{{ titulo }}</h2>
          <div id="paragrafos">
            <p id="p1">Last known location: {{ localizacao }}</p>
            <p id="p2">First seen in: {{ primeiroVisto }}</p>
          </div>
        </div>

        <!-- Gear Cop -->
        <div class="card">
          <img src="../assets/Personagens/gearcop.jpeg" alt="Imagem do card" />
          <h2>{{ titulo }}</h2>
          <div id="paragrafos">
            <p id="p1">Last known location: {{ localizacao }}</p>
            <p id="p2">First seen in: {{ primeiroVisto }}</p>
          </div>
        </div>

        <!-- Mechanical Summer -->
        <div class="card">
          <img src="../assets/Personagens/MechanicalSummer.jpeg" alt="Imagem do card" />
          <h2>{{ titulo }}</h2>
          <div id="paragrafos">
            <p id="p1">Last known location: {{ localizacao }}</p>
            <p id="p2">First seen in: {{ primeiroVisto }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- RODAPÉ -->
  <footer class="footer">
    <div class="rodape">
      <ul class="listaRodape">
        <li id="lista">CHARACTERS: </li>
        <li id="lista">LOCATIONS: </li>
        <li id="lista">EPISODES: </li>
      </ul>
      <p id="serverStatus">SERVER STATUS</p>
      <div class="servidores">

        <a id="servidor1" href="https://www.netlify.com/">
          <img id="imgServidores1" src="../assets/RedesSociais/netlify.png" alt="Netlify" style="max-width: 100%" />
          <h5 id="h5Servidores1">DEPLOYS BY</h5>
          <h4 id="h4Servidores1">netlify</h4>
        </a>
        <a id="servidor2" href="https://stellate.co/?ref=powered-by">
          <img id="imgServidores2" src="../assets/RedesSociais/Stellate.png" alt="Stellate" style="max-width: 100%;" />
          <h5 id="h5Servidores2">Powered by</h5>
          <h4 id="h4Servidores2">Stellate</h4>
        </a>

      </div>

      <div class="containerRS">
        <ul class="redeSocial">
          <li id="github"><a href="https://github.com/CaiioH/rick-and-morty" target="_blank"><img src="../assets/RedesSociais/github.png" alt="GitHub"
                style="max-width: 100%;" /></a></li>
          <li id="twitter"><a href="" target="_blank"><img src="../assets/RedesSociais/twitter.png" alt="Twitter"
                style="max-width: 100%;" /></a></li>
          <li id="suporte"><a href="" target="_blank"><img src="../assets/RedesSociais/coracao.png" alt="Suport"
                style="max-width: 100%;" /></a></li>
        </ul>
      </div>
      <div class="meuPerfil">
        <p id="pCaio">❮❯ by <a id="caioh" href="https://github.com/CaiioH?tab=repositories" target="_blank">Caio Henrique</a> 2024</p>

      </div>

    </div>

  </footer>

</template>
<script>


export default {
  name: 'MainCard',
  props: ['imagem', 'titulo', 'localizacao', 'primeiroVisto']
}



</script>

<style scoped>
body {
  margin: 0;
  padding: 0;
  border: none;
  overflow: hidden;
}
::selection{
  color: orange;
  background-color: black;
}

img {
  position: relative;
  max-width: 100%;
  width: 47%;
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  display: block;
  /* border: 1px solid orange; */
  /* margin:0; */
}

.containercard {
  /* border: 1px solid green; */
  background-color: rgb(39, 43, 51);
  /* background-color: red; */
  max-width: 100%;
  width: 100vw;
  /* height: 100vh; */
  display: flex;
  position: relative;
  justify-content: center;
  align-items: center;
  text-align: center;
  margin-top: -97px;

}

.allcards {
  max-width: 1920px;
  position: relative;
  /* border: 1px solid red; */
  margin: 0;
  padding: 10px;
  display: flex;
  background-color: rgb(39, 43, 51);
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 2px;
  right: 8px;

}

.card {
  /* margin: 1px; */
  margin: 0.75rem;
  /* width: 500px;
  height: 220px; */
  /* border: 1px solid green; */
  display: flex;
  background-color: rgb(60, 62, 68);
  color: white;
  border-radius: 0.5rem;
  padding-right: 128px;
  box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 6px -1px, rgba(0, 0, 0, 0.06) 0px 2px 4px -1px;
  overflow: hidden;
}

h2 {
  display: inline;
  position: absolute;
  /* border: 1px solid yellow; */
  margin-top: 15px;
  margin-bottom: 300px;
  margin-left: 235px;
  font-size: 1.5rem;
  font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
  font-weight: bold;
  color: rgb(255, 255, 255);
  cursor: pointer;
  /* border-bottom: none; */

}

h2:hover {
  color: orange;
}

#p1 {
  position: relative;
  /* border: 1px solid red; */
  font-size: 16px;
  font-weight: 500;
  margin: 10px;
  margin-bottom: 50px;
  text-align: left;
  padding: 0;
  color: rgb(158, 158, 158);
  font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
}

#p2 {
  position: relative;
  /* border: 1px solid red; */
  font-size: 16px;
  font-weight: 500;
  margin: 10px;
  padding: 0;
  color: rgb(158, 158, 158);
  font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
  text-align: left;
}

#paragrafos {
  position: relative;
  max-width: 100%;
  /* border: 1px solid orange; */
  margin: 0;
  margin-top: 70px;
  margin-bottom: 25px;
  margin-left: 5px;
}

.container {
  position: relative;
  display: flex;
  /* padding: 4.5rem 0px; */
  /* border: 1px solid blue; */
  /* background-color: blue; */
  width: 100vw;
  height: 61.0vh;
  margin-left: -9px;
  background-color: rgb(32, 35, 41);
}

.footer {
  /* border: 1px solid red; */
  background-color: rgb(32, 35, 41);
  margin-left: -9px;
  margin-bottom: -11px;
  width: 100vw;
  height: 370px;
  /* padding-top: 60px; */
  position:static;
  display:flex;
  overflow: hidden;
  justify-content: center;

}

.rodape{
  /* border: 1px solid red; */
  position: relative;
  top: 50px;
  display: block;
  overflow: hidden;


}

.listaRodape {
  position: relative;
  flex-direction: row;
  justify-content: center;
  display: flex;
  list-style: none;
  text-align: center;
  align-items: center;
  /* border: 1px solid orange; */
  padding: 5px;

}

#lista {
  position: relative;
  display: flex;
  padding: 1px;
  margin: 10px;
  /* border: 1px solid red; */
  color: rgb(158, 158, 158);
  opacity: 80%;
}

#lista:hover,
#serverStatus:hover,
#listaSocial:hover {
  color: orange
}

#serverStatus {
  /* border: 1px solid red; */
  color: rgb(158, 158, 158);
  opacity: 80%;
  margin: 15px;
  position: relative;
  top: -25px;
  text-align: center;
  bottom: 5px;
}

#serverStatus,
#lista,
.servidores,
#h5Servidores,
#h4Servidores {
  font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
  font-size: 13px;
  font-weight: bold;
  cursor: pointer;
  letter-spacing: 0.07mm;
}

/* Rodapé Servidores  */
.servidores {
  text-align: center;
  /* border: 1px solid blue; */
  display: flex;
  align-items: center;
  padding: 0;
  margin-right: 20px;
  margin-left: -30px;
  justify-content: center;
  position: relative;
  bottom: 45px;
  left: 25px
}

#servidor1 {
  position: relative;
  display: inline-flex;
  justify-content: center;
  /* border: 1px solid green; */
  gap: 5px;
  text-decoration: none;
  left: 50px;
  margin: 0;
  margin-top: 20px
}

#servidor2 {
  position: relative;
  display: inline-flex;
  justify-content: center;
  /* border: 1px solid red; */
  gap: 4px;
  font-style: none;
  text-decoration: none;
  left: 15px;
  margin: 0;
  margin-top: 20px
}

#imgServidores1 {
  margin-top: 15px;
  width: 33px;
  height: 33px;
  /* border: 1px solid green; */
  filter: brightness(2000%);
  position: relative;
  bottom: 2px;
  left: 2px;
}

#imgServidores2 {
  margin-top: 13px;
  width: 38px;
  height: 38px;
  /* border: 1px solid green; */
  opacity: 50%;
  filter: grayscale(5);
}
#imgServidores2::selection{
  background-color: rgba(0, 0, 0, 0.479);
}

#h5Servidores1 {
  /* border: 1px solid red; */
  font-size: 8px;
  color: rgb(158, 158, 158);
  font-style: none;
  letter-spacing: 0.3mm;
  font-weight: 500;
  position: relative;
  left: 1px;
  top: 2px;

}

#h4Servidores1 {
  position: relative;
  /* border: 1px solid yellow; */
  color: white;
  right: 60px;
  top: 1px;
  font-size: 17px;
  letter-spacing: 0.2mm;
  font-weight: 500;
}

#h5Servidores2 {
  /* border: 1px solid red; */
  position: relative;
  bottom: 3px;
  left: 3px;
  font-size: 11px;
  color: rgb(158, 158, 158);
  font-style: none;

}

#h4Servidores2 {
  position: relative;
  /* border: 1px solid yellow; */
  color: white;
  right: 63px;
  top: 3px;
  font-size: 18px;
  letter-spacing: 0.2mm;
  font-weight: 500;
}

/* --------------------- */
/* Rodapé Redes Sociais  */
#github,
#twitter,
#suporte {
  /* border: 1px solid red; */
  opacity: 50%;
  filter: invert();
  list-style: none;
}

.containerRS {
  /* border: 1px solid red; */
  justify-content: center;
  align-items: center;
  text-align: center;
  display: flex;
  padding: 0;
  margin: 0;
  position: relative;
  bottom: 25px;
  left: 10px;
  gap: 5px;

}

.redeSocial {
  /* border: 1px solid green; */
  margin: 0;
  padding: 0;
  justify-self: center;
  align-items: center;
  display: contents;
  position: relative;
}

#github {
  width: 40px;
}

#twitter {
  position: relative;
  top: 1px;
  width: 40px;
  left: 1px;
}

#suporte {
  width: 40px;
  position: relative;
  left: 1px;
}

/* ---------------------- */
/* Rodapé Meu Perfil  */
.meuPerfil {
  /* border: 1px solid rgb(223, 226, 41); */
  color: rgb(158, 158, 158);
  font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
  font-size: 13px;
  font-weight: bold;
  letter-spacing: 0.07mm;
  opacity: 80%;
  text-align: center;
  position: relative;
  bottom: 8px;

}

#caioh {
  color: white;
  font-weight: bold;
  text-decoration-color: orange;
  letter-spacing: 0.1mm;
  text-underline-position: under;
}
#pCaio{
  font-weight: normal
}

#caioh:hover,
.meuPerfil::selection {
  color: orange;
  text-decoration: none;

}

#github::selection{
  color: transparent;
  background-color: transparent;
}

#github:hover,
#twitter:hover,
#suporte:hover {
  opacity: 100%;
}
</style>
