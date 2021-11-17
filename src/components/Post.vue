<template>
  <div class="posts">
    <div class="content">
      <main>
    <div class="content-box" v-for = "post in postsList" :key="post.id" >
      <nav><div>Sep 18, 2020 15:16</div></nav>
      <div><h1>{{post.title}}</h1></div>
      <div><img class="image" src={{post.url}} alt="image"></div>
      <div class="text"><p>{{post.body}}</p></div>
    </div>
    <aside class="left-sidebar"></aside>
    <aside class="right-sidebar"></aside>
      </main>
    </div>
  </div>
</template>

<script>
export default {
  name: "Posts",
  data: function() {
    return {
    }},
  computed: {
    postsList(){
      return this.$store.state.postsList
    }}
};
</script>
<style scoped lang="css">
h1 {
  margin: 40px 0 0;
}
main {
  background: white;
  flex: 3;
  order: 2;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
.left-sidebar {
  order: 1;
  flex: 1;
}
.right-sidebar {
  flex: 1;
  order: 3;
}
.content {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}
.content-box {
  padding: 10px;
  margin-left: 80px;
  margin-right: 80px;
  margin-top: 10px;
  box-shadow: 0 0 5px 5px gainsboro;
  border-radius: 5px;
}
.image {
  width: 600px;
  margin: 0;
}
.text {
  margin-top: 5px;
  font-size: 20px;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}
.posts {
  margin-bottom: 150px;
}
</style>
