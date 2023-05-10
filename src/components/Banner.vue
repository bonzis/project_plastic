<template>
    <div class="banner"  :style="{ backgroundImage: 'radial-gradient(ellipse at center, rgba(27, 39, 53, 0) 0%, #090a0f 100%), url(' + imgUrlBanner + ')' }" >
        
        <h1 class="titlebanner">{{titleBanner}}</h1>
    </div>
</template>
<style>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@800&display=swap');

.banner
{
    display: flex;
    margin-top:90px;
    height: 500px;
    align-items: center;
    text-align: center;
} 
.titlebanner
{
    font-family: 'Manrope', sans-serif;
    margin: auto;
    color: white;
    text-align:center;
    font-size:7em;
    z-index: 3;
    text-shadow: #000000 3px 3px 3px;
    text-align: center;
    text-transform: uppercase;
}
</style>

<script setup>

const props = defineProps({
  titleBanner: String,
  imgUrlBanner:String,
})

</script>