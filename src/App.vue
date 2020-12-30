<template>
  <div id="app">
    <ejercicio-sidebar/>
  </div>
</template>

<script>
import EjercicioSidebar from './components/Sidebar.vue'

export default {
  name: 'App',
  components: {
    EjercicioSidebar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
