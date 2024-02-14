<script setup lang="ts">
import { onMounted } from 'vue';

const props = defineProps({
  title: String,
})

onMounted(() => { })
</script>

<template>
  <div class="title">{{ props.title }}</div>
</template>

<style lang="less" scoped>
.title {
  width: 100%;
  height: 52px;
  padding: 0px 24px;
  color: #787597;
  font-size: 16px;
  background-color: #F9FAFE;
  line-height: 52px;
  border-top: 1px solid #F3F2F8;
  border-bottom: 1px solid #F3F2F8;
  font-weight: bold;
}

[data-theme='dark'] {
  .title {
    color: #E0E4EB;
    background-color: #242B38;
    border: 1px solid #242B38;
  }
}
</style>