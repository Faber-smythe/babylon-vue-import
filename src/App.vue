<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <img alt="Babylon logo" src="https://www.babylonjs.com/assets/logo-babylonjs-social-twitter.png" />
  <img alt="Typescript logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Typescript_logo_2020.svg/1200px-Typescript_logo_2020.svg.png" />
  <h1>
    <a target="_blank" href="https://v3.vuejs.org/guide/introduction.html">Vue3</a> 
    + 
    <a target="_blank" href="https://www.babylonjs.com/">Babylon.js</a>
    + 
    <a target="_blank" href="https://www.typescriptlang.org/">Typescript</a>
  </h1>
  <HelloWorld msg="Asset from Mixamo.com" />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
}
#app>img{
  max-height: 120px;
  margin: 0px 15px;
}
#app>div{
  margin: 20px;
}
h1, h2, a{
  color: rgb(0, 162, 255);
}
a{
  text-decoration: none;
  transition: all 0.3s ease;
}
a:hover{
  opacity: 0.5;
}
</style>
