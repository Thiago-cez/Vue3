<template>
  
  <AlertComponente variant="danger" />
</template>

<script>
import AlertComponente from './components/AlertComponente.vue';


export default {
  name: 'App',
  components: {
    AlertComponente
},

  data() {
      
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
