<template>
  <div class="app-body">
    <!-- <h1 @click="count++">{{ count }}</h1> -->
    <h1 >{{ count }}</h1>
    <button @click="increment">Increment</button>
  </div>
</template>
<script>
import { ref } from 'vue'
  export default{
    setup(){
      const count = ref(0);
      function increment(){
        count.value= 6
      }
      return {
        count,
        increment
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


