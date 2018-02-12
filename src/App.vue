<template>
  <div id="app">
    <img src="./assets/logo.png">
    <Clock />
  </div>
</template>

<script>
import Clock from './components/Clock'

export default {
  name: 'App',
  components: {
    Clock
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  margin-top: 60px;
}
</style>
