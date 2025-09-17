<template>
  <div id="app">
    <Menu />
    <div class="content">
      <img alt="Vue logo" src="./assets/logo.png">
      <h1>Bienvenido a Vue.js</h1>
    </div>
  </div>
</template>

<script>
import Menu from './components/Menu.vue'

export default {
  name: 'App',
  components: {
    Menu
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
}

.content {
  margin-top: 80px;
}

</style>
