<template>
  <div id="app">
    <WebglFluid></WebglFluid>
    <test></test>
  </div>
</template>
<script>
import test from './components/test.vue'
import WebglFluid from './components/WebglFluid.vue'
export default {
  methods: {
    startHacking () {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  },
  components: {
    test,
    WebglFluid
  }
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
}
</style>
