<template>
  <div id="nav">
    <router-link class="nav-item" to="/">Home</router-link>
    <router-link class="nav-item" to="/about">About</router-link>
    <router-link class="nav-item" :to="{ name: 'Jobs' }">Jobs</router-link>
  </div>
  <div class="btn-group">
    <button @click="redirect">Redirect</button>
    <button @click="back">Go Back</button>
    <button @click="forward">Forward</button>
  </div>

  <router-view />
</template>

<script>
export default {
  name: 'App',
  components: {},
  methods: {
    redirect() {
      this.$router.push({ name: 'Home' });
    },
    forward() {
      this.$router.go(1);
    },
    back() {
      this.$router.go(-1);
    },
  },
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
.nav-item {
  margin: 10px;
  padding: 5px;
  border: 1px solid gray;
  text-decoration: none;
  border-radius: 5px;
  border-bottom: none;
}
.btn-group {
  margin: 20px;
}
button {
  margin: 0 10px;
  padding: 10px;
  border: none;
  border-radius: 4px;
}
</style>
