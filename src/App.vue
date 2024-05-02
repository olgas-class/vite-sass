<script>
import AppBanner from './components/AppBanner.vue';

export default {
  components: {
    AppBanner
  },
  data() {
    return {
      title: "Ciao"
    }
  }
}
</script>

<template>
  <h1 class="bg-black">{{ title }}</h1>
  <AppBanner />
  <h2>Ciao sono h2 di app</h2>
</template>

<style>
.bg-black {
  background-color: black;
  color: white;
}

/* h2 {
  color: red;
} */
</style>