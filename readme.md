# Vue 

> Vue JS, commonly referred to as Vue, is an open-source, progressive JavaScript framework created by Evan You in 2014 as an alternative to heavier frameworks like AngularJS and React. Vue combines Angular-influenced approaches and streamlined features for front-end interfacing and application development. Vue’s core library is focused on the view layer only and designed to be adopted into projects incrementally.

## Instalação do Vue CLI

- utilizado para executar o Vue Via linha de comando. Ex: executar comando para crear projetos verificar versão do vue e etc.

- utilizei o comando para instalar o Vue CLI globalmente: ( npm install -g @vue/cli )




## CLASS 2 
### CRIANDO O PROJETO VUE 

- Utilizei o comando para Criar nosso projeto: (vue create nomeDoProjeto)
### todo-app

### Project setup
```
npm install
```
### Compiles and hot-reloads for development
```
npm run dev
```
### Compiles and minifies for production
```
npm run build
```
### Lints and fixes files
```
npm run lint
```
### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## CLASS 3

#### Single File Component - SFC

- Vue Single-File Components (a.k.a. *.vue files, abbreviated as SFC) is a special file format that allows us to encapsulate the template, logic, and styling of a Vue component in a single file. Here's an example SFC:
   
```ruby
<script setup>
  import { ref } from 'vue'
  const greeting = ref('Hello World!')
</script>

<template>
  <p class="greeting">{{ greeting }}</p>
</template>

<style>
    .greeting {
        color: red;
        font-weight: bold;
    }
</style>
```

## CLASS 4
### Conditional Directive

 v-show
 v-if
 v-else-if
 v-else

## CLASS 5
### Directive Loops

 v-for

## CLASS 6
### Data Binding 

 v-bind 

## CLASS 7
### attributes Class and Dinamic Style

## CLASS 8
### two way data-bind

 v-model

## CLASS 9
### Directive

 v-on || @ => Short Format

## CLASS 10
### computed properties

computed: {
  
}

## CLASS 11
### watch - Observadores
//Usado para observar campos e fazer ações secundarias.
watch: {

}

## CLASS 12
### Life Cycle Hooks
  beforeCreate
  created
  beforeMount
  mounted
  beforeUpdate
  updated
  beforeUnmount
  unmounted

## CLASS 13
### Component slot

## CLASS 14
### Scoped e global css

## CLASS 15
### props
from father to child

## CLASS 16
### emits
from child to father

