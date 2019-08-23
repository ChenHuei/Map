<template>
  <div id="app">
    <Header/>
    <router-view :key="$route.fullPath"/>
  </div>
</template>

<script>
import Header from './components/Header'
export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">
@import "./styles/import";
#app {
  @include size(100vw, 100vh);
  font-size: 10px;
  font-family: $font-family;
  overflow: hidden;
}
</style>
