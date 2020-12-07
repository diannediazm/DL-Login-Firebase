<template>
  <div id="app">
    <div id="nav">
      <router-link to="/home">Home</router-link> |
      <router-link :to="{name: 'Login'}" class="login">Login</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style lang="scss">
#nav {
  text-align: center;
  margin: 10px 0px 10px 0px;
}
.router-link-exact-active {
  color: darkgrey;
}
.login {
  color: darkgrey;
}
</style>
