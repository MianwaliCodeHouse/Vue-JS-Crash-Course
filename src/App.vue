<template>
  <div class="app-body">
    <div v-if="userRole == 'admin'">(admin) this run when condtion true</div>
    <div v-else-if="userRole == 'user'">(user) this run when it's if condtion flase</div>
    <div v-else>(guest) this run when it's if condtion flase</div>
    <form @submit.prevent="onSubmit">
      <div class="">
        <input type="text" name="name">
      </div>
      <input type="submit" value="Submit">
    </form>
  </div>
</template>
<script>
export default{
  data(){
    return {
      userRole : 'guest'
      }
    },
    methods: {
      onSubmit(){
        
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


