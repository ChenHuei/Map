<template>
  <div id="app">
    <router-view :key="$route.fullPath"/>
  </div>
</template>

<script>

export default {
  name: 'App'
}
</script>

<style lang="scss">
@import "./styles/import";
#app {
  @include size(100vw, 100vh);
  display: flex;
  font-size: 10px;
  font-family: $font-family;
  overflow: hidden;
}
</style>
