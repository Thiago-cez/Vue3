<template>
  <TheHeader v-if="showHeader"/>
  <HelloWorld msg="Class4 App"/>

  <div v-if="estadoCondicao === 'admin'">
        <h1>AQUI VAI UM ADMINISTRADOR</h1>
    </div>

    <div v-else-if="estadoCondicao === 'user'">
        <h1>AQUI VAI UM USUARIO</h1>
    </div>
    
    <div v-else-if="estadoCondicao === 'owner'">
        <h1>AQUI VAI O DONO</h1>
    </div>

    <div v-else>AQUI VAI A SOBRA</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TheHeader from './components/TheHeader.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    TheHeader
  },

  data() {
       return {
        showHeader: true,
        estadoCondicao: "admin"
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
