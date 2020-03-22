<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src=https://static.retail.autofact.cl/img/logo-autofact-blanco.png
          transition="scale-transition"
          width="100"
        />
        <span>Prueba AUTOFACT</span>
      
      </div>
      <v-spacer></v-spacer>  


    </v-app-bar>

    <v-content>

      <HelloWorld/>
      <Registro/>
      <Preguntas/>

    </v-content>
  </v-app>



</template>

<script>
import HelloWorld from './components/HelloWorld';
import Registro from './components/login'
import Preguntas from './components/Preguntas'

export default {
  name: 'App',

  components: {
    
    Registro,
    HelloWorld,
    Preguntas,
  },

  data: () => ({
    //
  
  }),
};
</script>
