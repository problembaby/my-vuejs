<template >
  {{ msg || 'prop가 아직 전달 되지 않음' }}
</template>

<script>
export default {
  props:{
    msg: String
  }

}
</script>

<style>

</style>