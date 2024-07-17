<template>
  <div class="container">
    <div class="containercard">
          <!-- Morty -->
    <div class="card">
      <img src="../assets/Personagens/morty.jpeg" alt="Imagem do card"  />
      <h2>Titulo Grande pra caralho</h2>
      <div id="paragrafos">
        <p id="p1">Last known location: {{ localizacao }}</p>
        <p id="p2">First seen in: {{ primeiroVisto }}</p>
      </div>
    </div>

    <!-- Baby Rick -->
    <div class="card">
      <img src="../assets/Personagens/BabyRick.jpeg" alt="Imagem do card"  />
      <h2>{{ titulo }}</h2>
      <div id="paragrafos">
        <p id="p1">Last known location: {{ localizacao }}</p>
        <p id="p2">First seen in: {{ primeiroVisto }}</p>
      </div>
    </div>

    <!-- Roy's Son  -->
    <div class="card">
      <img src="../assets/Personagens/RoySon.jpeg" alt="Imagem do card"  />
      <h2>{{ titulo }}</h2>
      <div id="paragrafos">
        <p id="p1">Last known location: {{ localizacao }}</p>
        <p id="p2">First seen in: {{ primeiroVisto }}</p>
      </div>
    </div>

    <!-- Mechanical Rick  -->
    <div class="card">
      <img src="../assets/Personagens/MechanicalRick.jpeg" alt="Imagem do card"  />
      <h2>{{ titulo }}</h2>
      <div id="paragrafos">
        <p id="p1">Last known location: {{ localizacao }}</p>
        <p id="p2">First seen in: {{ primeiroVisto }}</p>
      </div>
    </div>

    <!-- Gear Cop -->
    <div class="card">
      <img src="../assets/Personagens/gearcop.jpeg" alt="Imagem do card"  />
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
  </template>
  <script>


  export default {
    name: 'MainCard',
    props: ['imagem', 'titulo', 'localizacao', 'primeiroVisto']
  }



  </script>
  
  <style scoped>
  body{
    margin:0;
    padding: 0;
    border:none;
  }
  /* .containercard{
    display: block;
    border: 1px solid red;
    margin: 50px 10px 50px 10px
  } */

  img{
    position: relative;
    max-width: 100%;
    width: 47%;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
    display: block;
    /* border: 1px solid orange; */
    /* margin:0; */
  }
    .container{
      max-width: 100%;
      width: 100%;
      height: 100%;
      position: absolute;
      margin: 50px;
      margin-bottom: 100%;
      margin-left: -8px;
      margin-top: -70px;
      border: 1px solid blue;
      padding: 70px 0px 70px 0px; 
      /* display: inline-block; */
      background-color: rgb(39, 43, 51);
      border-left: none;  
      text-align: center;  
      border-style: none;

    }

    .card {
      margin: 20px;
      /* border: 1px solid green; */
      display:inline-flex;
      background-color: rgb(60, 62, 68);
      color: white;
      border-radius: 10px;
      padding-right: 114px;
      text-align: left;
      /* padding-top: 20px; */
      
    }
    h2{
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
    h2:hover{
      color: orange;
    }

    #p1{
      position:relative;
      /* border: 1px solid red; */
      font-size: 16px;
      font-weight: 500;
      margin: 10px;
      margin-bottom: 50px;
      padding: 0;
      color: rgb(158, 158, 158);
      font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
    }

    #p2{
      position:relative;
      /* border: 1px solid red; */
      font-size: 16px;
      font-weight: 500;
      margin: 10px;
      padding: 0;
      color: rgb(158, 158, 158);
      font-family: 'BlinkMacSystemFont', 'Segoe UI', 'Roboto', 'Helvetica', 'Arial', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
    }

    #paragrafos{
      position:relative;
      /* display:block; */
      max-width: 100%;
      /* border: 1px solid orange; */
      margin: 0;
      margin-top: 70px;
      margin-bottom: 25px;
      margin-left: 5px;

      
    }
  
    
  </style>

