<template>
  <div class="tweet d-flex p-3 pb-2">
    <div class="circle p-0 border-0 me-2">
      <img class="profilePicture d-flex" src="../../../public/pp.png" />
    </div>
    <div class="body d-flex flex-column">
      <div class="top d-flex align-items-start">
        <h2 class="fs-6 name me-1 mb-0">Ozan Öztuna</h2>
        <h2 class="fs-6 hashtag me-1 mb-0">@ozanoztn</h2>
        <h2 class="fs-6 time hashtag mb-1">. 43d</h2>
        <button class="btn btn-more border-0">
          <i class="fa-solid fa-ellipsis fa-xl"></i>
        </button>
      </div>
      <p class="message pb-1 mb-0">Hello World!</p>
      <div class="intreaction d-flex justify-content-start">
        <div class="item d-flex align-items-center">
          <button class="btn border-0 p-2 d-flex" id="comments">
            <i class="fa-regular fa-comment"></i>
          </button>
          <h2 class="fs-6 p-0 m-0" id="comments-count">9</h2>
        </div>
        <div class="item d-flex align-items-center">
          <button class="btn border-0 p-2" id="retweets">
            <i class="fa-solid fa-retweet"></i>
          </button>
          <h2 class="fs-6 p-0 m-0" id="retweets-count">9</h2>
        </div>
        <div class="item d-flex align-items-center">
          <button class="btn border-0 p-2" id="likes">
            <i class="fa-regular fa-heart"></i>
          </button>
          <h2 class="fs-6 p-0 m-0" id="likes-count">9</h2>
        </div>
        <div class="item d-flex align-items-center">
          <button class="btn border-0 p-2" id="share">
            <i class="fa-solid fa-arrow-up-from-bracket"></i>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.circle {
  position: relative;
}
.profilePicture {
  border-radius: 50%;
  width: 55px;
  height: 55px;
}
.top {
  height: 1.3rem;
}
.hashtag {
  color: #676b6f;
}
.name {
  color: #dcdedf;
  font-weight: bold;
  width: 6.1rem;
}
.time {
  width: 2.3rem;
}
.message {
  font-weight: 400;
}
.btn {
  color: #2f3336;
  border-radius: 100%;
  height: 2.2rem;
  display: flex;
  justify-content: center;
  align-items: center;
}
.btn-more {
  color: #4d5054;
  height: 1.6rem;
  padding: 0.5rem !important;

  margin-left: 15.5rem;
}
.btn > i {
  font-size: 1.2rem;
}
h2 {
  transition: 300ms;
  color: #2f3336;
}
.item {
  margin-right: 5rem;
}
.item:hover > #comments,
.item:hover > #share,
.item:hover > #comments-count,
.btn-more:hover {
  color: #1b8bd7;
  background: #0a171f;
  transition: 300ms;
}
.item:hover > #retweets,
.item:hover > #retweets-count {
  color: #00ba7c;
  background: #071a14;
  transition: 300ms;
}
.item:hover > #likes,
.item:hover > #likes-count {
  color: #de1672;
  background: #200914;
  transition: 300ms;
}
</style>