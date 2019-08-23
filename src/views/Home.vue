<template>
  <div class="home">
    <googleMap/>
  </div>
</template>

<script>

import googleMap from '@/components/GoogleMap'

export default {
  name: 'home',
  components: {
    googleMap
  }
}
</script>

<style lang="scss" scoped>
@import "../styles/import";

.home {
  @include size(100vw, 100vh);
}
</style>
