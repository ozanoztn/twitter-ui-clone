<template>
  <div class="topic-container p-3 d-flex justify-content-between">
    <div>
      <div class="content mb-1">1.Gündemdekiler</div>
      <div class="topic">#Trend</div>
      <div class="tweet-count">33,6 B Tweet</div>
    </div>
    <button class="btn btn-more border-0">
      <i class="fa-solid fa-ellipsis fa-xl"></i>
    </button>
  </div>
</template>

<style scoped>
.topic-container:hover {
  background: #1d1f23;
  transition: 400ms;
}
.content {
  color: #71767b;
  font-size: 0.8rem;
}
.topic {
  color: white;
  font-weight: bold;
  font-size: 0.9rem;
}
.tweet-count {
  color: #595d62;
}
.btn-more {
  color: #4d5054;
  height: 2rem;
  padding: 0.5rem !important;
  border-radius: 999px;
  font-size: 0.7rem;
}
.btn-more:hover {
  color: #1b8bd7;
  background: #1d2c37;
  transition: 300ms;
}
</style>