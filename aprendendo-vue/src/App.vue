<template>
  <HelloWorld msg="Class4 App"/>
  
    <div>
    <h1> -- PRIMEIRO EXEMPLO -- </h1>
    <input id="inputField" v-model="teste1" placeholder="Digite algo aqui e veja a magica acontecer"><br>
    {{ teste1 }}

    </div><br>

    <div>
      <h1> -- SEGUNDO EXEMPLO -- </h1>
      <h4> -- LISTA DE ESCOLHA -- </h4>

      <label> Escolha um ESPORTE </label><br>
      <select v-model="teste2" value="">
        <option value="">Escolha</option>
        <option value="Futebol">Futebol</option>
        <option value="Handball">Handball</option>
        <option value="Volei">Volei</option>
        <option value="Natação">Natação</option>
        <option value="Corrida">Corrida</option>
        <option value="Judô">Judô</option>
        <option value="Tiro Livre">Tiro Livre</option>
        <option value="Baseball">Baseball</option>
        <option value="American Football">American Football</option>
      </select>

      <p> Voce escolheu: {{ teste2 }}</p>
    </div>

    <div>
      <h1> -- TERCEIRO EXEMPLO -- </h1>
      <h4> -- ESCOLHA VIA RADIO BUTTON -- </h4>

      <label> Gostas desse tipo de Exemplo </label><br>
       <input v-model="teste3" type="radio" value="SIM">SIM 
       <input v-model="teste3" type="radio" value="NÃO" >NÃO 

      <p> Voce escolheu: {{ teste3 }}</p>
    </div>

    <div>
      <h1> -- QUARTO EXEMPLO -- </h1>
      <h4> -- ESCOLHA VIA CHECK-BOX -- </h4>

      <label> FRUTARIA:  </label><br><br>
       <input v-model="frutaria" type="checkbox" value="BANANA"> Banana 
       <input v-model="frutaria" type="checkbox" value="MACA" > Maça 
       <input v-model="frutaria" type="checkbox" value="PERA" > Pera 
       <input v-model="frutaria" type="checkbox" value="KIWI" > Kiwi 
       <input v-model="frutaria" type="checkbox" value="UVA" > Uva 
       <input v-model="frutaria" type="checkbox" value="MELAO" > Melão  
       <input v-model="frutaria" type="checkbox" value="MANGA" > Manga
       <input v-model="frutaria" type="checkbox" value="MELANCIA" > Melancia 

      <p> Voce escolheu: {{ frutaria }}</p>
    </div>
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },

  data() {
       return {
         teste1: "Thiago Cezario",
         teste2: "",
         teste3: "",
         frutaria: []
       }
  }

}
</script>

<style>

#inputField {
  height: 30px;
  width: 300px;
  text-align: center;
  font-size: 20px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
