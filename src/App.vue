<template>
  <!---<img alt="Vue logo" src="./assets/logo.png"> -->
  <NavBar />
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  

  <div class="bg-red-500">
    Hey Tailwind
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import NavBar from './components/NavBar.vue';
import './assets/tailwind.css';
export default {
  name: 'App',
  components: {
    HelloWorld,
    NavBar
  }
}
</script>

<style>
#app {
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
