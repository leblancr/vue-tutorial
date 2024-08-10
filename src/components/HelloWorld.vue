<script setup lang="ts">
import { reactive, ref, defineProps } from 'vue'

// Define the props interface
interface Props {
  msg: string
}

const props = defineProps<Props>()  // Use defineProps with the Props type
const counter = reactive({ count: 0 })
const message = ref('Hello World!')  // initial value
console.log(counter.count) // "Hello World!"
console.log(message.value) // 0
counter.count = 1
message.value = 'Changed'
const titleClass = ref('title')

</script>

<template>
  <h1 :class="titleClass">{{ message }}</h1>
  <p>Count is: {{ counter.count }}</p>
  <span>Message: {{ props.msg }}</span>
</template>

<style scoped>
.title {
  color: red;
}
</style>
