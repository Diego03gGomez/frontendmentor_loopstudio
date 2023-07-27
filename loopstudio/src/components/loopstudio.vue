<template lang="">
    <div>
       



<div id="fondo1">
    <header>
<div class="cont_header">
<h1>loopstudio</h1>

<nav>
    <ul>
        <a href="">About</a>
        <a href="">Careers</a>
        <a href="">Events</a>
        <a href="">Products</a>
        <a href="">Suport</a>
    </ul>
</nav>
<div class="cont_oculto">
<a href="#">About</a>
<a href="#">Careers</a>
<a href="#">Events</a>
<a href="#">Products</a>
<a href="#">Suppor</a>
</div>



<i  v-on:click="trasladar()" class="fa-solid fa-bars menu"></i>
</div>
        </header>


<div class="cont_fondo1">

<h1>IMMERSIVE <br>
EXPERIENCES <br>
THAT DELIVER</h1>






</div>




</div>



<div id="fondo2">


<div class="cont_fondo2">
<div class="cont1_fondo2">
    <img src="https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/mobile/image-interactive.jpg" alt="">
</div>

<div class="cont2_fondo2">
    <h1>THE LEADER IN <br>
    INTERACTIVE VR</h1>
    <h4>Founded in 2011, Loopstudios has been produccing wolrd-class <br>
    virtual reality projects for some of the best companies around the <br>
globe. Our award-winning creating have transformed <br>
businesses through digital experiences that bind to their brand.</h4>
</div>



</div>

</div>


<div id="fondo3">

<div class="titulo_fondo3">
    <h1>OUR CREATIONS</h1>

    <a href="#">SEE ALL</a>
</div>


<div class="cont_cards">

<div v-for="(e, index) in imagenes" :key="index"  class="card">
    <img :src="e.img" alt="">
    <div class="cont_hover">
    <h1>{{e.titulo}}</h1>
</div>
</div>


</div>


</div>

<div class="boton_oculto">
    <a >SEE ALL</a>
</div>




<footer>


<div class="cont_footer">
<div class="columna1">
    <h2>loopstudios</h2>
<nav class="links" >
    <a href="#">About</a>
    <a href="#">Careers</a>
    <a href="#">Events</a>
    <a href="#">Products</a>
    <a href="#">Support</a>
</nav>

</div>


<div class="columna2">
    <div class="redes">
        <a href=""><i class="fa-brands fa-facebook"></i></a>
        <a href=""><i class="fa-brands fa-twitter"></i></a>
        <a href=""><i class="fa-brands fa-pinterest"></i></a>
        <a href=""><i class="fa-brands fa-instagram"></i></a>
    </div>
<h4>@2021 Loopstudios. All rights reserved.</h4>

</div>


</div>





</footer>



    </div>
</template>
<script>
export default {

data() {
    return {
        imagenes: [
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-deep-earth.jpg", titulo: "DEEP EARTH"},
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-night-arcade.jpg", titulo: "NIGHT ARCADE"},
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-soccer-team.jpg", titulo: "SOCCER TEAM VR"},
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-grid.jpg", titulo: "THE GRID"},
       
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-from-above.jpg", titulo: "FROM UP ABOVE"},
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-pocket-borealis.jpg", titulo: "NIGHT ARCADE"},
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-curiosity.jpg", titulo: "SOCCER TEAM VR"},
{img:"https://codelamp168.github.io/Loop-Studios-Landing-Page-Tailwind-React/imagelist/desktop/image-fisheye.jpg", titulo: "THE GRID"},
 

],

    }
},

methods: {
    trasladar() {
        let menu = document.querySelector(".cont_oculto");
        menu.classList.toggle("trasladar")
        
    }
},


    
}
</script>
<style lang="">
    
</style>