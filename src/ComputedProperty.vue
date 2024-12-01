<template>
  <div class="app-body">
    <!-- <h1 >Single Count: {{ count }}</h1>
    <h1 >Double Count: {{ doubleCount }}</h1> -->
    <!-- <button @click="increment">Increment</button> -->
     <h1>Author Publish Books?</h1>
     <h1>{{ answer }}</h1>
  </div>
</template>
<script>
import { computed, reactive, ref } from 'vue'
  export default{
    setup(){
      const author = reactive({
        name: 'John Doe',
        books: []
      })
      const answer = computed(()=>{
        return author.books.length > 0 ? "Yes" : "No";
      })
      // const count = ref(0);
      // function increment(){
      //   count.value++
      // }
      // const doubleCount = computed(()=>{ 
      //   return count.value*2;
      // });
      return {
        answer
        // count,
        // increment,
        // doubleCount
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


