<template>
  <mountedCompo></mountedCompo>
  <watchCompo></watchCompo>
  <childCop v-bind:msg="greeting"></childCop>
</template>

<script>
import mountedCompo from './components/mountedCompo.vue';
import watchCompo from './components/watchCompo.vue';
import childCop from './components/childCop.vue';

export default {
  name: 'App',
  components: {
    mountedCompo,
    watchCompo,
    childCop

  },
  data(){
    return{
      greeting : '부모 컴포넌트로 부터 prop 전달'
    }
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
