<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
      dark
    >
      <v-col cols="12" class="d-flex flex-column justify-space-between" style="height: 30rem">
        <v-col cols="12" class="d-flex  align-center flex-column">
          <v-btn width="235" to="./home" >read-me</v-btn>
          <v-btn width="235" to="./startgame" class="mt-3">start game</v-btn>
          <v-btn width="235" class="mt-3" to="./ponggame">pong game</v-btn>
        </v-col>
       
        <v-col cols="12" class="d-flex align-end " >
          <img src="./assets/top_img.png"> 
        </v-col>
        
      </v-col>
      
       
        
      
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