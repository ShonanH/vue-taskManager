<template>
  <div class="about-info">
    <h3>
      This is a Task Manager, aka A TO-DO List application made with hopes to
      compete against the likes of Trello
    </h3>
  </div>
  <router-link to="/">Home</router-link>
</template>

<style scoped>
div {
  background-color: rgb(2, 2, 2);
  height: 130px;
  width: 100%;
}
h3 {
  padding: 10px;
  justify-content: center;
  border-radius: 5px;
  color: rgb(245, 241, 241);
}

a {
  text-decoration: none;
  color: rgb(5, 5, 5);
  background-color: rgb(22, 225, 240);
  font-size: 1.1rem;
  border-radius: 5px;
  padding: 7px;
}
</style>
