<template>
  <p ref="p">안녕</p>

</template>

<script>
export default{
  mounted(){
    this.$refs.p.textContent = '마운트됨'
  }
}
</script>

<style>

</style>
