<template>
  <div class="container">
    <h3>User Start Component</h3>
    <hr />
    <ul class="list-group">
      <router-link class="list-group-item" to="/user/1" tag="li">
        <a>User 1</a>
      </router-link>
      <router-link class="list-group-item" to="/user/2" tag="li">
        <a>User 2</a>
      </router-link>
      <router-link class="list-group-item" to="/user/3" tag="li">
        <a>User 3</a>
      </router-link>
      <router-link class="list-group-item" to="/user/4" tag="li">
        <a>User 4</a>
      </router-link>
    </ul>
  </div>
</template>
<script>
export default {};
</script>
