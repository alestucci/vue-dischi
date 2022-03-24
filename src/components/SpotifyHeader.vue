<template>
  <header class="d-flex justify-content-between align-items-center">
    <div class="logo rounded-circle"></div>
    <select name="genre" id="genre">
      <option value="">Seleziona un genere</option>
      <option value="Rock">Rock</option>
      <option value="Pop">Pop</option>
      <option value="Jazz">Jazz</option>
      <option value="Metal">Metal</option>
    </select>
  </header>
</template>

<script>
export default {
  name: "SpotifyHeader",
};
</script>

<style lang="scss" scoped>
header {
  height: 70px;
  padding: 0 1rem;
  background-color: #2e3a46;
}
.logo {
  width: 50px;
  height: 50px;
  background-color: #1ed760;
}
</style>
