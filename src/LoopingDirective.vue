<template>
  <div class="app-body">
    <h1 v-for="number in numbers">{{ number }}</h1>
  </div>
</template>
<script>
  export default{
    data(){
      return {
        numbers : [11,22,33,44]
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


