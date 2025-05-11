<template>
  <!-- 通过bind一整个对象属性可以直接全部传入组件 -->
  <span>通过bind一整个对象属性可以直接全部传入组件</span>
  <AttributeDemo v-bind="objectOfAttrs" />
</template>

<script setup lang="ts">
import { reactive, ref } from 'vue'
import AttributeDemo from '@/components/AttributeDemo.vue'
const msg = ref('MSG')
const objectOfAttrs = reactive({
  data: 1,
  err: 'none',
  msg: 'test',
})
console.log(`output->msg`, msg)
</script>

<style></style>
