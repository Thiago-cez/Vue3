<template>
  
  <AlertComponente 
  :variant="variant" 
  @fechar="fecharAlerta()"
  v-if="showAlert"
  >{{ text}}</AlertComponente>
</template>

<script>
import AlertComponente from './components/AlertComponente.vue';


export default {
  name: 'App',
  components: {
    AlertComponente
},

  data() {

      return {
        showAlert: true,
        variant: "sucess",
        text: "Enviado com Sucesso"
      }      
    },
    methods: {
      fecharAlerta(){
        this.showAlert = false;
      }
    }
}
</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
