<template>
  <div>숫자변경될떄 콘솔에 기록</div>

  <div>할일 id : {{ todoId }}</div>
  <button v-on:click="todoId++">다음 할일 가져오기</button>
  <p v-if="!todoData">...로딩</p>
  <pre v-else>{{ todoData }}</pre>
  

</template>

<script>
export default {
  data(){
    return{
      todoId: 1,
      todoData:null,
    }
  },
  methods:{
    async fetchData(){
      this.todoData = null
      const res = await fetch(
        `https://jsonplaceholder.typicode.com/todos/${this.todoId}`
      )
      this.todoData = await res.json()
      console.log(res)
    }

  },

  
  mounted(){
    this.fetchData()
  },
  
  watch:{
    todoId(){
      this.fetchData()
    }
  }

}
</script>

<style>

</style>

