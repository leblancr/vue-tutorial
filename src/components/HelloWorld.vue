<script setup lang="ts">
import { ref } from 'vue'

const text1 = ref('')
const text2 = ref('')

</script>

<template>
  <input v-model="text1" placeholder="Type here1">
  <span>{{ text1 }}</span>
  <input v-model="text2" placeholder="Type here2">
  <p>{{ text1 }}</p>
  <span>{{ text2 }}</span>
</template>