<template>
  <div class="container">
    <router-view></router-view>
    <hr />
  
    <button class="btn btn-success" @click="navigateToHome">Home Component</button>
    <button class="btn btn-primary" @click="navigateToHome1">Home Component</button>
    <button class="btn btn-info" @click="navigateToHome2">Home Component</button>
  </div>
</template>
<script>
  export default {
    data(){
      return {
        id : this.$route.params.id
      }
    },
    methods : {
      navigateToHome(){
        this.$router.push("/");
      },
      navigateToHome1(){
        this.$router.push({path : '/'});
      },
      navigateToHome2(){
        this.$router.push({name : 'anasayfa'});
      },
    },
    watch : {
      "$route" (to, from){
        this.id = to.params.id;
      }
    }
  }
</script>
