<template>
  <div id="app">
    <span>24123123</span>
    <el-button type="primary">默认按钮</el-button>
    <router-view/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      a: 1,
      b: '123'
    }
  },
  methods: {
    test () {
      console.log(this.b)
    }
  },
  mounted () {
    console.log(this.a);
    console.log(this.test());
  }
})
</script>
<style lang="scss" scoped>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: $warning-color
  }
</style>
