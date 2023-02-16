<template>
  <div class="col-6 p-3 px-0">
    <div class="d-flex justify-content-between align-items-center px-3">
      <h4>Anasayfa</h4>
      <i class="fa-regular fa-star btn fs-5 border-0"></i>
    </div>
    <div class="tweet d-flex mt-3 px-3">
      <div class="circle p-0 border-0 me-3">
        <img class="profilePicture d-flex" src="../../../public/pp.png" />
      </div>
      <div class="tweetInput d-flex flex-column">
        <textarea
          class="border-0 form-control fs-5 mb-1"
          cols="70"
          rows="2"
          placeholder="Neler Oluyor ?"
          v-model="tweet"
        ></textarea>
        <div class="bottom d-flex justify-content-between">
          <div class="tweet-options d-flex">
            <button class="btn border-0 p-0 buttom-button">
              <i class="fa-regular fa-image"></i>
            </button>
            <button class="btn border-0 p-0 buttom-button">
              <i class="fa-solid fa-gift"></i>
            </button>
            <button class="btn border-0 p-0 buttom-button">
              <i class="fa-solid fa-square-poll-horizontal"></i>
            </button>
            <button class="btn border-0 p-0 buttom-button">
              <i class="fa-regular fa-face-smile"></i>
            </button>
            <button class="btn border-0 p-0 buttom-button">
              <i class="fa-solid fa-calendar-check"></i>
            </button>
            <button class="btn border-0 p-0 buttom-button" disabled>
              <i class="fa-solid fa-location-dot"></i>
            </button>
          </div>
          <button class="tweetButton btn border-0" :disabled="!tweet">
            Tweetle
          </button>
        </div>
      </div>
    </div>
    <Tweet />
    <Tweet />
    <Tweet />
    <Tweet />
  </div>
</template>
<script>
import Tweet from "../Tweet.vue";
export default {
  data() {
    return {
      tweet: "",
    };
  },
  components: {
    Tweet,
  },
};
</script>
<style scoped>
.col-6 {
  border: 1px solid #2f3336;
  color: #e7e9ea;
  width: 37.5rem;
}
.fa-star {
  color: white;
  border-radius: 50%;
  padding: 0.7rem;
}

.fa-star:hover {
  background: #181818;
}
.tweetInput > textarea {
  background: #000;
}
.circle {
  position: relative;
}
.profilePicture {
  border-radius: 50%;
  width: 55px;
  height: 55px;
}
.form-control {
  resize: none;
  color: white;
}
.tweet {
  border-bottom: 1px solid #2f3336;
}
.buttom-button {
  color: #1a8cd8;
  border-radius: 100%;
  padding: 0.7rem !important;
  height: 2.5rem;
  display: flex;
}
.buttom-button:hover {
  background: #031018;
}
.tweetButton {
  color: white;
  background: rgb(0 152 255);
  border-radius: 999px;
  text-align: center;
  height: max-content;
  width: 6rem;
}
.tweetButton:hover {
  background: #1a8cd8;
}
</style>