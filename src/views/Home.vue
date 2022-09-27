<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">  
    <h1>Hello, this is VueJs and Vuex Journal Practice</h1>
    <p>Here are examples of it, click on Daybook for test it</p>  
    <button @click="goToDayBook" class="btn btn-primary">DayBook</button>
    <button class="btn btn-secondary">Secondary</button>
    <button class="btn btn-success">Success</button>
  </div>
</template>


<script>
export default {
  methods:{
    goToDayBook() {
      this.$router.push({name:'no-entry'})
    }
  }
}
</script>

<style lang="scss" scoped>
  .home{
      border-bottom: 1px solid #198754;
      background-color: lighten($color: grey, $amount:0);
      height: 100vh;
      width: 100vw;
  }
</style>
