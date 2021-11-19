<template>
  <div>
    <button @click="Testing">Reset likes</button>
  </div>
</template>

<script>
export default {
  name: "ResetButton",
  components: {},
  methods: {
    Testing: function() {
      for (let i = 0; i < this.$store.state.postsList.length; i++) {
        this.$store.state.postsList[i].count = 0
      }
    }
  }
};
</script>

<style scoped></style>
