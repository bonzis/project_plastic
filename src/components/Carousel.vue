<template>
    <v-carousel class="carousel"
    v-bind:cycle="true"
    show-arrows="hover"
   hide-delimiter-background
   color="white"
>
        <v-carousel-item 
        class="imgCarousel"
        
          src="../../public/img/plamontagna.jpg"
          cover
        >
        <div class="imgtext">
          <h2>INFOGRAFICA</h2>
          <p>Gruppo 123 </p>
        </div>
      </v-carousel-item>

      <v-carousel-item 
        class="imgCarousel"
        
          src="../../public/img/1294117.png"
          cover
        >
        <div class="imgtext">
          <h2>LOGO</h2>
          <p>Gruppo 123 </p>
        </div>
      </v-carousel-item>

      <v-carousel-item 
        class="imgCarousel"
        
          src="../../public/img/tappi.jpg"
          cover
        >
        <div class="imgtext">
          <h2>FUMETTO</h2>
          <p>Gruppo 123 </p>
        </div>
      </v-carousel-item>
      
      </v-carousel>
  </template>
  <style>
  .v-carousel-item
  {
    position:relative;
    height: 100vh;
  }
 
  .imgtext 
  {
    z-index:3;
    color:white;
    font-weight: bold;
    text-shadow: #000000 3px 5px 2px;
    position:absolute;
    top:70%;
    left:0;
    padding-left:30px;
    
    
  }
  .imgtext p
  {
    font-size:20px;
  }
  .imgtext h2
  {
    font-size:90px;
  }
</style>