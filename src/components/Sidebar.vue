<template>
  <div class="sidebar">
    <input type="text">
  </div>
</template>

<script>
export default {
  name: 'Sidebar'
}
</script>

<style lang="scss" scoped>
@import "../styles/import";
.sidebar {
  @include size(20rem, 100%);
}
</style>
