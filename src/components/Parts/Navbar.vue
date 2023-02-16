<template>
  <div class="col-3 d-flex flex-column justify-content-between">
    <div class="d-flex flex-column">
      <NavButton
        className="fa-brands fa-twitter fa-2xl twitterBrandIcon me-4"
      />
      <NavButton className="fa-solid fa-house fa-xl me-4" text="Anasayfa" />
      <NavButton className="fa-solid fa-hashtag fa-xl me-4" text="Keşfet" />
      <NavButton className="fa-solid fa-bell fa-xl me-4" text="Bildirimler" />
      <NavButton className="fa-solid fa-envelope fa-xl me-4" text="Mesajlar" />
      <NavButton
        className="fa-solid fa-bookmark fa-xl me-4"
        text="Yer İşaretleri"
      />
      <NavButton className="fa-solid fa-list fa-xl me-4" text="Listeler" />
      <NavButton className="fa-solid fa-user fa-xl me-4" text="Profil" />
      <NavButton
        className="fa-solid fa-ellipsis fa-xl me-4"
        text="Daha Fazla"
      />

      <button class="tweetButton btn border-0">Tweetle</button>
    </div>

    <div
      class="
        profileBox
        btn
        d-flex
        justify-content-between
        align-items-center
        p-3
        border-0
      "
    >
      <div class="d-flex">
        <div class="circle me-3">
          <img class="profilePicture d-flex" src="../../../public/pp.png" />
        </div>
        <div class="userInfos d-flex flex-column align-items-start">
          <h2 class="fs-6 m-0 name">Ozan Öztuna</h2>
          <h2 class="fs-6 hashtag">@ozanoztn</h2>
        </div>
      </div>
      <i class="fa-solid fa-ellipsis"></i>
    </div>
  </div>
</template>

<script>
import NavButton from "../NavButton.vue";
export default {
  components: {
    NavButton,
  },
};
</script>

<style scoped>
.col-3 {
  width: 270px;
}
.tweetButton {
  margin-top: 2rem;
  font-size: 1.2rem;
  color: white;
  background: rgb(0 152 255);
  border-radius: 999px;
  text-align: center;
  padding: 0.7rem 0 0.7rem 0;
}
.tweetButton:hover {
  background: #1a8cd8;
}
.profileBox {
  color: white;
  border-radius: 999px;
}
.profileBox:hover {
  background: #181818;
}
.circle {
  border-radius: 50%;
  overflow: hidden;
}
.profilePicture {
  width: 50px;
  height: 50px;
}
.hashtag {
  color: #676b6f;
}
.name {
  color: #dcdedf;
}
</style>