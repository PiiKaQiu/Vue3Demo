<template>
  <span>{{ data }}</span>
  <span>{{ msg }}</span>
  <span>{{ err }}</span>
</template>

<script setup lang="ts">
const props = defineProps(['data', 'msg', 'err'])
console.log(`output->data`, props)
</script>

<style></style>
