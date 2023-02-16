<template>
  <div :class="basicClass">
    <i :class="className"></i>
    <h2 class="m-0">
      {{ text }}
    </h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      basicClass: "btn d-flex align-items-center py-3 pe-4",
    };
  },
  props: ["className", "text"],
  methods: {
    twitterBrand() {
      this.text
        ? (this.basicClass = this.basicClass)
        : (this.basicClass = this.basicClass + " twitterBrand");
    },
  },
  created() {
    this.twitterBrand();
  },
};
</script>

<style scoped>
.btn {
  color: white;
  max-width: max-content;
  border-radius: 999px;
  border: 0;
  font-size: 0.9rem;
}
.btn:hover {
  background: #181818;
}
i {
  width: 25px;
}
h2 {
  font-size: 1.3rem;
}
.twitterBrand {
  margin-bottom: 0.2rem;
  border-radius: 100%;
  max-width: max-content;
  padding-right: 0.7rem !important;
}
.twitterBrand:hover {
  background: #031018;
}
.twitterBrandIcon {
  margin-right: 0 !important;
  width: 34px;
  height: 25px;
  padding: 0.8rem 0 0.8rem 0 !important;
  border-radius: 50%;
}
</style>