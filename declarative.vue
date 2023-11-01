<script setup>
import { ref,reactive } from 'vue'

const message = ref('Hello World!')
const counter = reactive({
  count: 0
})
console.log(counter.count) // 0
counter.count++
</script>

<template>
  <h1>{{ message.split('').reverse().join('') }}</h1>
  <input v-model="msg">
  <p>count is: {{ counter.count }}</p>
</template>