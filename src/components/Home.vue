<template>
  <div class="container">
    <h3>Home Component</h3>
    <hr>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis, earum libero odit optio repellendus sed
      soluta? Animi, atque blanditiis commodi consequatur distinctio dolorem eaque eos expedita, modi reprehenderit
      repudiandae soluta.
    </p>
    <hr>
    <button class="btn btn-success" @click="navigateToUser">User Component</button>
    <button class="btn btn-primary" @click="navigateToUser1">User Component</button>
  </div>
</template>
<script>
  export default {
    methods : {
      navigateToUser(){
        this.$router.push('/user/13');
      },
      navigateToUser1(){
        this.$router.push({ path : '/user/22'});
      },

    }
  }
</script>
