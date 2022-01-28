<template>
  <h1>Vue.js Components Fundamentals</h1>
  <ButtonCounter />
  <ButtonCounter />
  <ButtonCounter />
  <ButtonCounter />
</template>

<script>
import ButtonCounter from './components/ButtonCounter.vue'

export default {
  name: 'App',
  components: {
    ButtonCounter
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
