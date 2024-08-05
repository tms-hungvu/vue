<script setup lang="ts">
const emit = defineEmits(['click-decrement'])
const getEventDecrement = () => {
  emit('click-decrement')
}
</script>
<template>
  <button @click="getEventDecrement()">-</button>
</template>
