<template >
    <div class="ciao"   >
        
        <v-container   class="product-container" >
            
            <v-row align="center" >
                <v-col v-for="ciaos in ciao"  align="center"   >
                    <Prodotto  title="Logo" authors="Il logo del progetto!" imgUrl="../../public/img/logo.png" />
                    <Prodotto  title="Infografica" authors="Una breve infografica che racconta il mondo della sostenibilità \n, mantenendo il focus sullo spreco della plastica" imgUrl="../../public/img/1294117.png" />
                    <Prodotto  title="Fumetto" authors="Un fumetto che sfrutta un contesto divertente per fungere da denuncia per quanto riguarda lo spreco della plastica" imgUrl="../../public/tappi.jpg" />
                </v-col>
            </v-row>
        </v-container>
      
        
        
    </div>
</template>

<script setup>
import Prodotto from '@/components/Prodotto.vue';

</script>

<style >


.ciao
{
    background-color: #81D4FA;
    padding-top: 200px ;
    height: 100vh;
}  
.v-row .v-col 
{
    
    justify-content:center;
}

</style>