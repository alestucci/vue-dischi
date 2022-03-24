<template>
  <header class="d-flex justify-content-between align-items">
    <div class="logo"></div>
    <select name="genre" id="genre">
      option*
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
  background-color: #2e3a46;
}
.logo {
  width: 50px;
  height: 50px;
  background-color: #1ed760;
}
</style>
