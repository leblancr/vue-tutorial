<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="app-container">
    <HelloWorld msg="Hello World!" />
  </div>
</template>

<style scoped>
.app-container {
  min-height: 100vh; /* Ensure it covers the full viewport height */
}
</style>
