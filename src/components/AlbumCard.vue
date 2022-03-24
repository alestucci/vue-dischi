<template>
  <div>
    <div class="card text-center">
      <img
        src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg"
        alt="Album"
      />
      <h2 class="py-3 fs-5">New Jersey</h2>
      <h3 class="fs-5 fw-light">Bon Jovi</h3>
      <h4 class="fs-5 fw-light pb-4">1988</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "AlbumCard",
};
</script>

<style lang="scss" scoped>
.card {
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
