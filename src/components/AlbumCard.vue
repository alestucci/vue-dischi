<template>
  <div>
    <div class="card text-center">
      <img :src="albumData.poster" :alt="albumData.title" />
      <h2 class="py-3 fs-5">{{ albumData.title }}</h2>
      <h3 class="fs-5 fw-light">{{ albumData.author }}</h3>
      <h4 class="fs-5 fw-light pb-4">{{ albumData.year }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "AlbumCard",
  props: {
    albumData: Object,
  },
};
</script>

<style lang="scss" scoped>
.card {
  min-height: 420px;
  background-color: #2e3a46;
  padding: 1rem;
}
h2 {
  color: white;
}
h3,
h4 {
  color: grey;
}
</style>
