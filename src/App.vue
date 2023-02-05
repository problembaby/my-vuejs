<template>
  <mountedCompo></mountedCompo>
</template>

<script>
import mountedCompo from './components/mountedCompo.vue'

export default {
  name: 'App',
  components: {
    mountedCompo

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
