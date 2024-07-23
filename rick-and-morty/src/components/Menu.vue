<template>
  <nav class="Menu">
    <img id="img" src="../assets/svgs/logo.png" alt="Logo">
    <ul>
      <li><a id="docs" href="#docs">Docs</a></li>
      <li><a id="about" href="#about">About</a></li>
      <li><a id="sup" href="#support">SUPPORT US</a></li>
    </ul>
  </nav>
  <div class="Th1">
    <img id="titulo" src="../assets/svgs/The_rick_and_Morty_API.png" alt="Titulo">
    <!-- <br> -->
    <!-- <br> -->
    <h1>The Rick and Morty API</h1>
  </div>
</template>

<script>
export default {
  name: 'MainMenu'
}
</script>

<style scoped>
body {
  margin: 0;
  padding: 0;
  top: 0;

}
::selection{
  color: orange;
  background-color: black;
}


.Menu {
  display: flow-root;
  /* border: 1px solid green; */
}

a {
  color: rgb(36, 36, 36);
  list-style: none;
  text-decoration: none;
  font-size: 18px;
  font-weight: bold;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

/* quando o mouse tiver em cima */
#sup:hover {
  background-color: orange;
  color: white;
  transition: 0.1s;
}

/* quando o mouse tiver em cima */
#docs:hover,
#about:hover {
  color: orange;
  transition: 0.1s;
}

ul {
  position: relative;
  float: right;
  list-style: none;
  padding-inline: 0px;
  max-width: 100%;
  margin-top: -3px;
  right: 3px;
  /* border: 1px solid red; */

  /* margin-right: 25px; depois que a pagina estiver completa, tirar essa linha */


}

li {
  float: left;
  padding: 16px;
  /* border: 1px solid blue; */
}

img {
  float: left;
  max-width: 100%;
  width: 97px;
  margin-left: -10px;
  margin-top: -3px;
  cursor: pointer;
  position: absolute;
  /* border: 1px solid orange; */
}

#docs,
#about {
  position: relative;
  left: 2px;
  bottom: 4px;
}


#sup {
  /* bottom: auto; */
  margin-bottom: 15px;
  border-width: 1px;
  border-style: solid;
  border-color: orange;
  border-radius: 9px;
  padding: 9px 17px 8px 17px;
  font-size: 14px;
}

.Th1 {
  position: relative;
  display: flex;
  /* margin-top: -70px; */
  /* border: 1px solid green; */
  /* background-color: green; */
  justify-content: center;
  text-align: center;
  align-items: center;
  flex-wrap: wrap;
  /* max-width: 1920px; */
  min-width: 25%;
}

#titulo {
  position: relative;
  display: flex;
  /* border: 1px solid red; */
  min-width: 20%;
  width: 415px;
  padding: 0px;
  padding-bottom: 40px;
  opacity: calc(5%);
  cursor: default;
  left: 597px;
  bottom: 16px;

}

h1 {
  /* border: 1px solid blue; */
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  bottom: 60px;
  right: 10.7%;
  display: flex;
  text-align: center;
  letter-spacing: 0.07mm;
  font-size: 6.300rem;
  position: relative;
  font-weight: 900;
  font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
}

h1::selection {
  background-color: black;
  color: orange;
}
</style>