<template>
  <li>
    <img :src="imgUrl" :alt="title" />
    <a :href="url"> {{ title }} </a>
  </li>
</template>

<script>
export default {
  name: "CardItem",
  mounted: function () {
    if (this.imgUrl) {
      this.image = this.imgUrl;
    }
    this.loading = false;
  },
  data() {
    return {
      image: null,
      loading: true,
    };
  },
  props: ["title", "url", "imgUrl"],
};
</script>

<style scoped lang="scss">
li {
  width: calc(100% / 5);
  color: white;
  img {
    height: 50px;
    margin-right: 1em;
    vertical-align: middle;
  }
  a {
    text-transform: uppercase;
  }
}
</style>
