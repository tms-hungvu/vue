<script setup lang="ts">
import { ref } from 'vue'
import DecrementView from './DecrementView.vue'
import IncrementView from './IncrementView.vue'
const count = ref(0)
const increment = () => {
  count.value++
}
const decrement = () => {
  count.value--
}
</script>

<template>
  <main>hello world {{ count }}</main>
  <DecrementView @click-decrement="decrement()" />
  <IncrementView :count="count" @click-increment="increment" />
</template>
