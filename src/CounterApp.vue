<template>
  <div class="app-body">
    <h3>Counter App</h3>
    <h1>{{ count == 0 ? 'Start Counting by button' : count }}</h1>
    <button @click="increment">Click here to Increment Value</button>
  </div>
</template>
<script>
export default{
  data(){
    return {
      count : 0
    }
  },
  methods: {
    increment(){
      ++this.count; 
    }
  }
}
</script>
<style>
.app-body{
  text-align: center;
  padding: 30px;
}
</style>


