<template>
  <div id="nav">
    <router-link class='nav-item' to="/">Home</router-link>
    <router-link class='nav-item' to="/about">About</router-link>
    <router-link class='nav-item' :to="{name: 'Jobs'}">Jobs</router-link>
  </div>
  <router-view />
</template>

<script>
export default {
  name: 'App',
  components: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.nav-item{
  margin:10px;
  padding:5px;
  border:1px solid gray;
  text-decoration:none;
  border-radius:5px;
}
</style>
