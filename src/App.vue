<template>
  <div id="app">
    <Menu />
    <cuerpo></cuerpo>
    <Footer />
  </div>
</template>

<script>
import Cuerpo from './components/Cuerpo.vue'
import Footer from './components/Footer.vue'
import Menu from './components/Menu.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Cuerpo,
    Footer,
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
