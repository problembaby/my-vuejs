<template >
  <h2>자식컴포넌트</h2>
  {{ msg || 'prop가 아직 전달 되지 않음' }}

</template>

<script>
export default {
  // emit할 이벤트 선언
  emits:['response'],
  created(){
    //인자와 함께 emit
    this.$emit('response','자식 컴포넌트 부터 emit 발송')
  },
  props:{
    msg: String
  },


}
</script>

<style>
  
</style>