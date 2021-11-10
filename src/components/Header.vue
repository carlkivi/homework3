<template>
  <div>
    <h2>Header component</h2>
    <nav id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/contactus">Contact Us</router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
h2 {
  color: darkgreen;
}
</style>
