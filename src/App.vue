<template>
  <div id="app">
    <image_component height="100" width="100"/>
  </div>
</template>

<script>
import image_component from './components/image.vue'

export default {
  name: 'App',
  components: {
    image_component
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
