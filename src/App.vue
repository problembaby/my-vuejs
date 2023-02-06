<template>
  <mountedCompo></mountedCompo>
  <watchCompo></watchCompo>
</template>

<script>
import mountedCompo from './components/mountedCompo.vue';
import watchCompo from './components/watchCompo.vue';

export default {
  name: 'App',
  components: {
    mountedCompo,
    watchCompo

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
