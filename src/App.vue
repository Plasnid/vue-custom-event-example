<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Clickydoo @goTime="goActions" />
  </div>
</template>

<script>
import Clickydoo from './components/Clickydoo'

export default {
  name: 'App',
  components: {
    Clickydoo
  },
  methods: {
    goActions(e) {
      console.log("go actions has been called");
      console.log(e);
    }
  },
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
