<template>
  <div class="home">
    <h1>This is a home page</h1>
  </div>
  <Post></Post>
</template>

<script>
// @ is an alias to /src
import Post from "@/components/Post";
export default {
  name: "Home",
  components: { Post },
};
</script>
