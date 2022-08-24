<template>
  <canvas ref="canvas"/>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import WebglFluid from 'https://unpkg.com/webgl-fluid@0.1.0/dist/webgl-fluid.es.js'
const canvas = ref(null)

onMounted(() => {
  WebglFluid(document.querySelector(canvas.value))
})
</script>

<style>
canvas {
  width: 100vw;
  height: 100vh;
}
</style>
