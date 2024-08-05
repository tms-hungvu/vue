<script setup lang="ts">
defineProps(['count'])
const emit = defineEmits(['click-increment'])
const getEventIncrement = () => {
  emit('click-increment')
}
</script>
<template>
  <div :style="{ color: 'red', display: 'flex', gap: '5px' }">
    <span class="">value currently in component children : {{ count }}</span>
    <button @click="getEventIncrement()">+</button>
  </div>
</template>
