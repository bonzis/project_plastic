<template>
   
<v-card
    class="cardlearn"
    width="100%"
    max-height="600px"
    card-actions-flex=true
  >
  <v-row
    
  >
    <v-col>
      <v-img
        :src="img"
        height="600px"
        width="800px"
        cover
        float="left"
        
      ></v-img>
    </v-col>
    <v-col>
    <v-card-title class="title">
     {{ utitolo }}
    </v-card-title>

    <v-divider class="border-opacity-75"></v-divider>

        <v-card-text class="text">
            {{ testo }}
        </v-card-text>
      </v-col>
      </v-row>
  </v-card>

</template>

<script setup >
const props = defineProps({
  utitolo: String,
  testo:String,
  img:String,
})

</script>

<style scoped>
.cardlearn
{
  border: 50px;

}
.title
{
  font-size:100px;
}
.text
{
  text-align:center;
}
/*.subtitle
{
  padding:10px 0;
}*/
</style>