<template>
  <nav class="header">
    <div class="left">
      eFoood
    </div>
    <div class="right">
      <ul>
        <li>
          <el-select v-model="language">
            <el-option
              v-for="lang in language_array"
              :key="lang.locale"
              :value="lang.locale"
              :label="lang.name">
            </el-option>
          </el-select>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
import { LAND_RESPONSE } from '../constants'
export default {
  name: 'Header',
  data () {
    return {
      language: 'zh-tw',
      language_array: LAND_RESPONSE.locale
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../styles/import";

.header {
  @include size(100%, 56px);
  @include flexCenter;
  justify-content: space-between;
  padding: 8px 16px;
  background-color: color(grey);
}

ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
</style>
