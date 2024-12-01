<template>
  <div class="app-body">
    <h3>Counter App</h3>
    <p :id="dynamic_id">dynamic id</p>
    <h1 v-bind="objAttr">Dynamically Binding Multiple Attributes</h1>
  </div>
</template>
<script>
export default{
  data(){
    return {
      dynamic_id : 'r1',
      objAttr : {
        id : 'container',
        class : 'random-class',
        style : 'color: red'
      }
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


