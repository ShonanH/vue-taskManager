<template>
  <footer>
    <p>Copyright &copy; 2021</p>
    <router-link v-show="aboutPage" to="/about">About Me</router-link>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  computed: {
    aboutPage() {
      if (this.$route.path === "/") {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>

<style scoped>
a {
  text-decoration: none;
  color: rgb(5, 5, 5);
  background-color: rgb(22, 225, 240);
  font-size: 1.1rem;
  border-radius: 5px;
  padding: 7px;
}

p {
  margin-bottom: 10px;
}

footer {
  margin-top: 25px;
  color: aliceblue;
  text-align: center;
}
</style>
