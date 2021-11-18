<template>
  <div class="home">
    <h1>This is a home page</h1>
    <reset-button></reset-button>
  </div>
  <Post></Post>
</template>

<script>
// @ is an alias to /src
import Post from "@/components/Post";
import ResetButton from "@/components/ResetButton";
export default {
  name: "Home",
  components: { ResetButton, Post },
  /*
  computed: {
    postsList(){
      return this.$store.state.postsList
    }},
   */
};
</script>
