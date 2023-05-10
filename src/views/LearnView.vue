<template>

<div class="learnView">
    <h1 class="title">IMPARA</h1>
    <v-container class="card">
        <v-row>
                <CardLearn utitolo="COSA È LA PLASTICA E LA SUA STORIA" testo="lorem lorem lorem lorem lorem lorem lorem lorem lorem " img="../../public/img/tappi.jpg" />
                <CardLearn utitolo="I TIPI DI PLASTICA VANTAGGI E SVANTAGGI" testo="lorem lorem lorem lorem lorem lorem lorem lorem lorem " img="../../public/img/tappi.jpg" />
                <CardLearn utitolo="CICLO DI VITA DELLA PLASTICA" testo="lorem lorem lorem lorem lorem lorem lorem lorem lorem " img="../../public/img/tappi.jpg" />
                <CardLearn utitolo="ISOLE DI PLASTICA" testo="lorem lorem lorem lorem lorem lorem lorem lorem lorem " img="../../public/img/tappi.jpg" />
                <CardLearn utitolo="LA MICROPLASTICA" testo="lorem lorem lorem lorem lorem lorem lorem lorem lorem " img="../../public/img/tappi.jpg" />
                <CardLearn utitolo="LA PLATICA MONOUSO" testo="lorem lorem lorem lorem lorem lorem lorem lorem lorem " img="../../public/img/tappi.jpg" />
          
        </v-row>
    </v-container>
 </div>   
</template>
<script setup>
    import CardLearn from '@/components/CardLearn.vue';


</script>
<style>
.learnView
{
  background-color:#81D4FA;
  height:100%;
  /*
  5ADBFF
  1FCEFF
  0ACAFF
  https//coolors  
  https//colorhu/
  */
/*
#F6F1F1
#19A7CE
#146C94
#000000
*/
/*
#00FFF6
#00E7FF
#009EFF
#0014FF
*/
/*
#EFFFFD
#B8FFF9
#85F4FF
#42C2FF
*/

/*
https//fonts.g.com/specimen/Press+Start+2P?preview.text=IL%20RICICLAGGIO&preview.text_type=custom
per pagina riciclo che sta bene con i sprite del gioco
*/


}
.title
{
    font-size: 150px;
    padding: 200px;
    text-align:center; 
    color:#006aff;
}    
</style>