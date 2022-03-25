<template>
  <main>
    <div class="container">
      <h1 v-if="albumsArray === null" class="text-center">
        Dati in caricamento
      </h1>
      <div
        v-else
        class="row row-cols-sm-2 row-cols-md-3 row-cols-lg-4 row-cols-xl-5 gy-3 gx-5"
      >
        <h1>{{ genreProp }}</h1>
        <album-card
          v-for="album in albumsArray"
          :key="album.title"
          :album-data="album"
        />
      </div>
    </div>
  </main>
</template>

<script>
import AlbumCard from "./AlbumCard.vue";
import axios from "axios";

export default {
  name: "SpotifyMain",
  data() {
    return {
      albumsArray: null,
    };
  },
  components: {
    AlbumCard,
  },
  props: {
    genreProp: String,
  },
  created() {
    setTimeout(() => {
      axios
        .get("https://flynn.boolean.careers/exercises/api/array/music")
        .then((response) => {
          this.albumsArray = response.data.response;
        });
    }, 2000);
  },
};
</script>

<style lang="scss" scoped>
main {
  min-height: calc(100vh - 70px);
  padding: 5rem 0;
  background-color: #1e2d3b;
}
h1 {
  color: white;
}
</style>
