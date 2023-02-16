<template>
  <div class="container">
    <div class="row">
      <Navbar />
      <Tweets />
      <Topics />
    </div>
  </div>
</template>

<style scoped>
.row {
  height: 100vh;
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
</style>

<script>
import Navbar from "./components/Parts/Navbar.vue";
import Tweets from "./components/Parts/Tweets.vue";
import Topics from "./components/Parts/Topics.vue";
export default {
  components: { Navbar, Tweets, Topics },
};
</script>