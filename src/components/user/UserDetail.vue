<template>
  <div class="container">
    <h3>User Detail Component</h3>
    <hr />
    <p>Kullanıcı Id : {{ $route.params.id }}</p>
    <hr />
    <router-link
      tag="button"
      class="btn btn-danger"
      :to="{name : 'userEdit',
          params : { id : this.$route.params.id },
          query : {name : 'Alex', lastName : 'De Souza'},
          hash : '#data'}"
      >Edit</router-link>
  </div>
</template>
<script>
export default {
  beforeRouteEnter(to, from, next){
      console.log("Component Seviyesinde Kontrol!!!");
      next();
    }
};
</script>
