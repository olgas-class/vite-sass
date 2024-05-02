<script>
export default {
  data() {
    return {
      imageNum: "1",
      nature:
        "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwallup.net%2Fwp-content%2Fuploads%2F2016%2F03%2F10%2F318375-nature-landscape-lake-mountain-forest-wildflowers-spring-pine_trees-path-Switzerland-HDR.jpg&f=1&nofb=1&ipt=64d63718655aa9cbecc840ab7b83bb3cb0ca90d9b8c5484f62229a1ff4b2f7f3&ipo=images",
    };
  },
  methods: {
    getImageUrl(imageName) {
      return new URL(`../assets/img/meme-${imageName}.jpg`, import.meta.url)
        .href;
    },
  },
};
</script>

<template>
  <div class="banner">
    <h2 class="bg-black">Titolo</h2>
  </div>
  <div>
    <!-- <img src="/img/flowers.jpg" alt="">
    <img src="../assets/img/class.jpg" alt=""> -->

    <!-- <img :src="getImageUrl(imageNum)" alt="" />

    <img :src="nature" alt=""> -->
  </div>
</template>

<style scoped>
.banner {
  height: 60vh;
  background-color: lightblue;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

h2 {
  color: greenyellow;
}
</style>
