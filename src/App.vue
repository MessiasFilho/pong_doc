<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
      dark
    >

      <v-col class="ml-6 mt-6">
        <v-row>
        <img src="./assets/top_img.png"> 
      </v-row>  

      </v-col>
      <v-col class="mt-6 ml-3 mr-3">
      
      <v-row>
        <v-btn width="235" to="./home" >read-me</v-btn>
      </v-row>

      <v-row>
        <v-btn width="235" to="./startgame" class="mt-3">start game</v-btn>
      </v-row>

      <v-row>
        <v-btn width="235" class="mt-3" to="./ponggame">pong game</v-btn>
      </v-row> 

      </v-col>
      <div class="d-flex align-start flex-column mb-6">
       
      </div>
       
        
      
      </v-navigation-drawer>
      <v-app-bar dark app>
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Documentação</v-toolbar-title>
      </v-app-bar>
    
    <v-main  >
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>
  
  export default {
    name: 'App',
    data: () => ({ drawer: null }),
  }
</script>

<style lang="css">
.theme--dark.v-data-table tbody tr:nth-of-type(even) {
    background-color: rgba(85, 85, 85, 0.5);
}

</style>