<template>
    <nav class="Menu">
      <img id="img" src="../assets/svgs/logo.png" alt="Logo">
      <ul>
        <li><a id="docs" href="#docs">Docs</a></li>
        <li><a id="about" href="#about">About</a></li>
        <li><a id="sup" href="#support">SUPPORT US</a></li>
      </ul>         
    </nav>
    <nav class="Th1">
        <img id="titulo" src="../assets/svgs/The_rick_and_Morty_API.png" alt="Titulo">
        <br>
        <br>
        <h1>The Rick and Morty API</h1>
      </nav>
  </template>
  
  <script>
  export default {
    name: 'MainMenu'
  }
  </script>
  
  <style scoped>
  body{
    margin:0;
    padding:0;
    top:0;
  }
  .Menu{
    display:flow-root
  }
  a{
    color: rgb(36, 36, 36);
    list-style: none;
    text-decoration: none;
    font-size: 18px;
    font-weight: bold;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
  }
  /* quando o mouse tiver em cima */
  #sup:hover{  
    background-color: orange;
    color: white;
    transition: 0.1s;
  }

  /* quando o mouse tiver em cima */
  #docs:hover, #about:hover{  
    color: orange;
    transition: 0.1s;
  }

  ul{
    float:right;
    list-style: none;
    padding-inline: 0px;
    max-width: 100%; 
    margin-top: -5px;
    margin-right: 25px; /*depois que a pagina estiver completa, tirar essa linha */
    

  }
  li{
    float: left;
    padding:16px;
    /* border: 1px solid blue; */
  }

  img{
    float: left;
    max-width: 100%;
    width: 97px;
    margin-left: -10px;
    margin-top: -3px;
    cursor: pointer;
    position:fixed;
  }

  #sup{
    /* bottom: auto; */
    margin-bottom: 15px;
    border-width: 1px;
    border-style: solid;
    border-color:orange;
    border-radius: 9px;
    padding: 8px;
    padding-left: 16px;
    padding-right: 16px;
    font-size: 14px;
  }
  .Th1{
    margin-top: -70px;
  }

  #titulo{
    max-width: 100%;
    width: 400px;
    margin:auto;
    margin-top: 53px;
    margin-left: 38%;
    /* position: relative; */
    opacity:calc(5%)
  }

  h1{
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    display: block;
    text-align:center;
    margin: 200px;
    margin-top: 150px;
    /* margin-left: 15%; */
    margin-right: 10%;
    font-size: 105px;
    position:relative;
    font-weight: bold;
    font-family:'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
  }
  h1::selection{
    background-color: black;
    color: orange;
  }


  </style>