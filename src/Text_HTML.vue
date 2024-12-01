<template>
  <div class="app-body">
    <h3>Counter App</h3>
    <p>{{ vue_variable }}</p>
    <p v-html="vue_variable"></p>
  </div>
</template>
<script>
export default{
  data(){
    return {
      vue_variable : '<span style="color: red">This should be red.</span>'
    }
  },
}
</script>
<style>
.app-body{
  text-align: center;
  padding: 30px;
}
</style>


