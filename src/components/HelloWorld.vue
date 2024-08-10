<script setup>
import { reactive, ref } from 'vue'

const counter = reactive({ count: 0 })
const message = ref('Hello World!')  // initial value
console.log(counter.count) // "Hello World!"
console.log(message.value) // 0
counter.count = 1
message.value = 'Changed'
</script>

<template>
  <h1>{{ message }}</h1>
  <p>Count is: {{ counter.count }}</p>
</template>

<style scoped>

</style>
