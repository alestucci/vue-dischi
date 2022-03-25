<template>
  <div>
    <spotify-header @genre="genreFilter" />
    <spotify-main :genre-prop="genrePropString" />
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
  data() {
    return {
      genrePropString: "",
    };
  },
  methods: {
    genreFilter(genreString) {
      this.genrePropString = genreString;
    },
  },
};
</script>

<style lang="scss">
@import "./assets/styles/styles.scss";
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
