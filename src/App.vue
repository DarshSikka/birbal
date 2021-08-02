<template>
  <div id="nav">
    <router-link to="/">घर</router-link> |
    <router-link to="/about">बारे में</router-link> |
    <router-link to="/contact">संपर्क</router-link> |
    <router-link to="/idea">विचार</router-link>
  </div>
  <router-view />
  <Footer />
</template>
<script>
import Footer from "@/components/Footer";
export default {
  components: {
    Footer,
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
}

#nav {
  padding: 30px;
  display: flex;
  justify-content: space-around;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
