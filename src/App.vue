<template>
  <div id="app">
    <Adv></Adv>
  </div>
</template>

<script>
import Adv from './components/Adv.vue'

export default {
  name: 'App',
  components: {
    Adv
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
