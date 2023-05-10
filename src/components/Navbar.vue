
<template > 
    
   <v-app-bar  class="nav"  color="#B3E5FC" :height='90' :elevation="10" >
    <v-app-bar-nav-icon id="hamburger" @click.stop="drawer = !drawer" ></v-app-bar-nav-icon>
    <img id ="logores" class="logo"
            
            src="img/logo.png"
            
            
            />
    <ul class="bar" >
        <li><v-btn class="button" :ripple="false" v-for="btn in menu1btn "><router-link :to="btn.link">{{btn.name}}</router-link></v-btn></li>
       <li>
            <img class="logo" 
            
            src="img/logo.png"
            
            
            />
       </li>

        <li>
        
          <v-menu
          transition="slide-y-transition"
            class="learnMenu"
          >
            <template v-slot:activator="{ props }">
              <v-btn
                color="primary"
                v-bind="props"
              >
                Learn
              </v-btn>
            </template>

            <v-list>
              <v-list-item
                v-for="(item, i) in items"
                :key="i"
              >
                <v-list-item-title><router-link :to="item.link" >{{item.title}}</router-link></v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>
        
          <v-btn class="button" :ripple="false" v-for="btn in menu2btn "><router-link :to="btn.link" >{{btn.name}}</router-link></v-btn>
        </li>
    

    </ul>  
    </v-app-bar>
    <v-navigation-drawer
    id="limenu"
    v-model="drawer"
    location="left"
    temporary
    width="50%"
  >
    <v-list>
      
      <v-list-item v-for="btn in menu1btn">
        <v-list-item-title><router-link :to="btn.link">{{btn.name}}</router-link></v-list-item-title>
      </v-list-item>
      <v-list-item v-for="btn in menu2btn">
        <v-list-item-title><router-link :to="btn.link">{{btn.name}}</router-link></v-list-item-title>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
   
  
</template>


<style>
.learnMenu
{
  text-align:center;
}

.nav
{
    z-index: initial;
}

#hamburger{
    display:none;
}

#logores
{ 
  margin:auto;
  position:relative;
  display:none;
}

#limenu
{
   display:none;
   width: 50%;
   height: 100%;
   text-align:center;
}

.limenu:hover
{
    background-color:grey;
}

.bar
{
    list-style-type: none;
    width:100vw;
    height:auto;
    padding:10px;display:flex;
    justify-content: space-between;
    align-items: center;
}

.logo
{
  max-width:70px;
}

.bar li  
{
  padding:30px; 
}

a
{   
    color:#1867BF;
    text-decoration: none;
}


@media only screen and (max-width:675px) {

    #hamburger{display:inline-block;}
    .bar
    {
        display:none;
    } 
    #limenu{display:block;}
    #logores{display:block;}
}

</style>
<script setup>
  import { ref } from 'vue';
  
  let drawer = ref(false);
  const menu1btn = [{name:"HOME",link:"/"},{name:"PRODUCTS",link:"/products"}]
  const menu2btn = [{name:"LEARN",link:"/learn"},{name:"ABOUT US",link:"/about"}]

  const items= [{title:"COSA È LA PLASTICA E LA SUA STORIA",link:'/historyplastic'},
                {title:"I TIPI DI PLASTICA VANTAGGI E SVANTAGGI",link:'/typeplastic'},
                {title:"CICLO DI VITA DELLA PLASTICA",link:'#'},
                {title:"ISOLE DI PLASTICA",link:'#'},
                {title:"LA MICROPLASTICA",link:'#'},
                {title:"LA PLATICA MONOUSO",link:'#'},
                {title:"IL RICICLAGGIO",link:'#'},
                ]
</script>
