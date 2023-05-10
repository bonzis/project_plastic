<template>

<div class="learnView">
    <h1 class="title">IMPARA</h1>
    <v-container class="card">
        <v-row>
            <v-col v-for="ciaos in ciao"  
             
             
             >
                <CardLearn :utitolo="ciaos.titolo" :testo="ciaos.testo" :img="ciaos.img" />
            </v-col>
        </v-row>
    </v-container>
 </div>   
</template>
<script setup>
    import CardLearn from '@/components/CardLearn.vue';

import { ref } from 'vue';

const ciao=[
    {
        titolo:"COSA È LA PLASTICA E LA SUA STORIA", testo:"dodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"
    },
    {
        titolo:"CICLO DI VITA DELLA PLASTICA",testo:"dsoasiodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"
    },
    {
        titolo:"IL CICLO DI VITA DELLA PLASTICA",testo:"dodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"
    },
    {
        titolo:"LE ISOLE DI PLASTICA",testo:"dodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"
    },
    {
        titolo:"LA MICROPLASTICA",testo:"dodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"
    },
    {
        titolo:"LA PLATICA MONOUSO",testo:"dodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"
    },
    {
        titolo:"IL RICICLAGGIO s",testo:"dodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvasdodiosodosidoasdoidaoisdoiaodsoioadosaidosodioasiodioidovasiodvas",img:"../../img/tappi.jpg"    
    },
    
]
</script>
<style>
.learnView
{
  background-color:#81D4FA;
  height: 100%;
  /*
  5ADBFF
  1FCEFF
  0ACAFF
  https://coolors.co/
  https://colorhunt.co/
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
https://fonts.google.com/specimen/Press+Start+2P?preview.text=IL%20RICICLAGGIO&preview.text_type=custom
per pagina riciclo che sta bene con i sprite del gioco
*/


}
.title
{
    font-size: 150px;
    padding: 200px;
    text-align: center;
    color: #006aff;
}

</style>