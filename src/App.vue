<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" width="40" height="40">
    <button @click="toggle = !toggle">Toggle Sandbox</button>
    <sand-box v-if="toggle" />1
  </div>
</template>

<script>
import SandBox from './components/sandbox.vue'
export default {
  name: 'App',
  components: {
    SandBox
  },
  data: () => ({
    toggle: true,
  }),
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
