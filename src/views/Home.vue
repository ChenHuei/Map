<template>
  <div class="home">
    <Header/>
    <div class="container">
      <Sidebar/>
      <googleMap/>
    </div>
  </div>
</template>

<script>

import Header from '@/components/Header'
import Sidebar from '@/components/Sidebar'
import googleMap from '@/components/GoogleMap'

export default {
  name: 'home',
  components: {
    Header,
    Sidebar,
    googleMap
  }
}
</script>

<style lang="scss" scoped>
@import "../styles/import";

.home {
  @include size(100%);
  > .container {
    @include size(100%, calc(100% - 56px));
    @include flexCenter;
  }
}
</style>
