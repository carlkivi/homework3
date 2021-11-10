<template>
  <div id="app">
    <Header id="header"></Header>
    <router-view />
    <Footer id="footer"></Footer>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
}
#header {
  min-height: 50px;
  background: lightcyan;
}
#footer {
  background: PapayaWhip;

  bottom: 0;
  width: 100%;
  height: 120px; /* Height of the footer */
  position: fixed;
}
</style>
<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";
export default {
  components: { Footer, Header },
};
</script>
