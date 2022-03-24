<template>
  <main>
    <div class="container">
      <div
        class="row row-cols-2 row-cols-md-3 row-cols-lg-4 row-cols-xl-5 gy-3 gx-5"
      >
        <album-card />
        <album-card />
        <album-card />
        <album-card />
        <album-card />
        <album-card />
        <album-card />
        <album-card />
        <album-card />
        <album-card />
      </div>
    </div>
  </main>
</template>

<script>
import AlbumCard from "./AlbumCard.vue";

export default {
  name: "SpotifyMain",
  components: {
    AlbumCard,
  },
};
</script>

<style lang="scss" scoped>
main {
  height: calc(100vw - 70px);
  padding: 5rem;
  background-color: #1e2d3b;
}
</style>
