<template>
  <div id="app">
    <myTitle />
  </div>
</template>

<script>
import myTitle from './components/Title.vue'

export default {
  name: 'App',
  components: {
    myTitle,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
