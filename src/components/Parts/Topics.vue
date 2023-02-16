<template>
  <div class="col-3 pt-2 ps-4">
    <div class="searchBar d-flex align-items-center">
      <i class="fa-solid fa-magnifying-glass fa-lg"></i>
      <input type="text" class="search border-0" placeholder="Twitter'da Ara" />
    </div>
    <div class="topics">
      <h5 class="topics-header px-3 pt-3">Türkiye gündemleri</h5>
      <topic />
      <topic />
      <topic />
      <topic />
      <topic />
      <topic />
      <topic />
    </div>
  </div>
</template>

<script>
import topic from "../topic.vue";
export default {
  components: {
    topic,
  },
};
</script>

<style scoped>
.col-3 {
  width: 24.15rem;
}
.searchBar {
  background: #202327;
  border-radius: 999px;
  padding: 0.5rem 1.2rem 0.5rem 1.2rem;
}
.searchBar:focus-within {
  border: 1px solid #1a8cd8;
}
.searchBar:focus-within > i {
  color: #1a8cd8;
}
.fa-magnifying-glass {
  color: #676c71;
}
.search {
  background: #202327;
  margin-left: 1rem;
  caret-color: white;
}
.search:focus {
  outline: none;
}
.topics {
  background: #16181c;
  margin-top: 1rem;
  border-radius: 1rem;
  overflow: hidden;
}
.topics-header {
  color: white;
  font-weight: bold;
}
</style>