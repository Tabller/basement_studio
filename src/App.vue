<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <HelloWorld msg="Basement Studio" class="title" />
</template>

<style scoped>
.title {
  will-change: filter;
  transition: filter 300ms;
}
.title:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
</style>
