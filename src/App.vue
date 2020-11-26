<template>
  <div>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Landing</title>
    <link rel="stylesheet" href="estilos.css">
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@300&display=swap" rel="stylesheet">
  <div>
  <header>
    <div class="container">
      <nav>
        <a href="#" id="icono" class="icono">Menú</a>
        <div class="enlaces uno" id="enlaces">
          <a href="">Inicio</a>
          <a href="">Acerca de</a>
          <a href="">Contacto</a>
        </div>
      </nav>
      <div class="textos">
        <h1>MINIMARKET</h1>
        <h2>Hacemos la web ideal para ti</h2>
        <a href="#">Contacto</a>
      </div>
      <img src="src/assets/calculator.svg" alt="">
    </div>
  </header>
  <div class="wave">
    <div style="height: 150px; overflow: hidden;" ><svg viewBox="0 0 500 150" preserveAspectRatio="none" style="height: 100%; width: 100%;"><path d="M-9.93,-12.53 C175.16,239.10 337.69,-135.89 505.30,71.34 L500.00,150.00 L0.00,150.00 Z" style="stroke: none; fill: rgb(255, 255, 255);"></path></svg></div>
  </div>
  </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: { },
  methods: {
    navSlide() {
    const burger = document.querySelector('.burger');
    console.log(burger);
    const nav = document.querySelector('.nav-links');
    console.log(nav);
    nav.classList.toggle('nav-action');
    burger.classList.toggle('toggle');
}
  }
}

</script>

<style scoped>
*{
  margin:0;
  padding: 0;
  box-sizing: border-box;
}

body{

  font-family: 'Raleway', sans-serif;
}

nav{
  position: fixed;
  top: 20px;
  left: 20px;
  display: flex;
  justify-content: flex-start;
}

nav a{
  color:#fff;
  text-decoration: none;
}

.icono{
  display: block;
  z-index: 100000000;
  animation: moverIzquierda 1s ease-in;
}

header{
  background: #DA4453;
  background: -webkit-linear-gradient(to right, #89216B, #DA4453);
  background: linear-gradient(to right, #89216B, #DA4453);
  height: auto;
  padding: 48px;
  width: 100%;
}

.container{
  width: 95%;
  max-width: 1200px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin: auto;
}

img{
  display: block;
  height: 450px;
  object-fit: cover;
  animation: arriba 1s ease-in;
}

.textos{
  width: 50%;
  color:#fff;
}

.textos h1{
  font-size:80px;
  animation: moverDerecha 1s ease-in;

}

.textos h2{
  font-size:30px;
  animation: moverIzquierda 1s ease-in;
}

.textos a{
  display: inline-block;
  color:#fff;
  font-weight: 300;
  text-decoration: none;
  margin-top: 30px;
  border: 1px solid #fff;
  width: 150px;
  border-radius: 3px;
  text-align: center;
  padding: 10px 0;
  animation: arriba 1s ease-in;

}

.wave{
  height: 100px;
  width: 100%;
  background: #DA4453;
  background: -webkit-linear-gradient(to right, #c42597, #DA4453);
  background: linear-gradient(to right, #89216B, #DA4453);
}

.enlaces{
  position: fixed;
  display: flex;
  top: 0;
  background: #000;
  justify-content: space-around;
  align-items: center;
  height: 100vh;
  right: 0;
  flex-direction: column;
  width: 100%;
  transition: all 1s ease;
  background: #bc4e9c;
  background: -webkit-linear-gradient(to right, #be3261, #bc4e9c);
  background: linear-gradient(to right, #f80759, #e6aa3b);

}

.uno{

  -webkit-clip-path: circle(0% at 0 0);
  clip-path: circle(0% at 0 0);

}

.dos{

  -webkit-clip-path: circle(150% at 0 0);
  clip-path: circle(150% at 0 0);

}

</style>
