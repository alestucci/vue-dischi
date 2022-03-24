<template>
  <div>
    <spotify-header />
    <spotify-main />
  </div>
</template>

<script>
import SpotifyHeader from "./components/SpotifyHeader.vue";
import SpotifyMain from "./components/SpotifyMain.vue";

export default {
  name: "App",
  components: {
    SpotifyHeader,
    SpotifyMain,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
