<template>
  <div id="app">
    <!-- Navigation Bar -->
     <div id="bootstrap-overrides">
      <!-- Navigation Bar -->
      <nav class="navbar mynav">
        <div class="col-lg-2.1 shadow" style="cursor: pointer;" onclick="window.location='/';">
          <h4 class="differ1">Minimarketaa</h4>
        </div>
          <ul class="nav-links">
             <li>
                <a href="/terms&conditions">Terminos y condiciones</a>
             </li>
          </ul>

            <div class="col-lg-2.1 shadow2" style="cursor: pointer;" onclick="window.location='/terms&conditions';">
              <h4 class="differ2">Marco Legal</h4>
            </div>
      </nav>

    <section class="zoom">
        <!-- Router View -->
        <div class="container mt-3">
          <router-view/>
        </div>
      </section>
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
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

body {
    background-color: white;
}

h1 {
    color: white;
    font-size: 100px;
    font-family: 'Cabin', sans-serif;
}

p {
    color: black;
    text-align: justify;
    display: flex;
    width: 90%;
    letter-spacing: 2px;
    font-family: 'Cabin', sans-serif;
    padding: 15px;

}
/*Menú arriba*/
#bootstrap-overrides nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    min-height: 8vh;
    font-family: 'Cabin', sans-serif;
  background-color: rgb(0, 102, 255, 0.0);
    position: fixed;
    top: 0;
    width: 100%;
}

#bootstrap-overrides .navbar {
    -webkit-box-shadow: 0 8px 6px -6px #ffffff;
    -moz-box-shadow: 0 8px 6px -6px #ffffff;
    box-shadow: 0 8px 6px -6px #cacaca;
    z-index: 1000;
}

#bootstrap-overrides .logo {
    color: #a95a5a;
    letter-spacing: 3px;
    font-size: 26px;
}

#bootstrap-overrides .nav-links {
    display: flex;
    justify-content: space-around;
    width: 45%;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

#bootstrap-overrides .nav-links li {
    list-style: none;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

#bootstrap-overrides .nav-links a{
    text-decoration: none;
    color: #ffffff;
    /* font-weight: bold; */
    font-size: 18px;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}

#bootstrap-overrides .burger {
    display: none;
    cursor: pointer;
}

#bootstrap-overrides .burger div{
    width: 20px;
    height: 2px;
    background-color: black;
    margin: 5px;
    transition: all 0.3s ease;
}

.differ1{
  color: rgb(0, 102, 255, 0.0);
  letter-spacing: 2px;

}

.shadow{
  margin-right: 1320px;
  margin-top: 15px;
}
.shadow2{
  margin-left: 1300px;
}
@media screen and (max-width:1024px){
    #bootstrap-overrides .nav-links {
       width: 50%;
   }

}

    body {
        overflow-x: hidden;
    }

    /*Menú desplegable*/
    #bootstrap-overrides .nav-links{
        position: absolute;
        right: 0px;
        height: 92vh;
        top: 8vh;
        background-color: #ca2323;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 10%;
        transform: translateX(100%);
        transition: transform 0.3s ease-in;
        z-index: 101;
    }

    #bootstrap-overrides .nav-links a {
        color: black;
        opacity: 100%;
    }

    #bootstrap-overrides .burger {
        display: block;
    }

    .zoom #layer1 {
        height: auto;
    }

    .zoom #layer2 {
        height: auto;
    }



#bootstrap-overrides .nav-action {
    transform: translateX(0%);
}

.zoom{
    width: 100%;
    height: 100%;
    position: fixed;
    background: url(assets/minibg.png);
    background-size: 1600px
}
</style>
