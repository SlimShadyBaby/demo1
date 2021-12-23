<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <hello-world msg="Welcome to Your Vue.js App"/>
    <demo msg="my first demo" />
    <computed />
    <css />
  </div>
</template>

<script>
import Computed from './components/Computed.vue'
import Css from './components/Css.vue'
import Demo from './components/Demo.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    Demo,
    HelloWorld,
    Computed,
    Css
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
