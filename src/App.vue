<script setup lang="ts">
import type { ConfigProviderTheme } from 'vant'
// import { useStore } from '@/stores'

// const store = useStore()
const theme = ref<ConfigProviderTheme>('light')
// const mode = computed(() => store.mode)

// watch(mode, () => {
//   // 始终设定为light模式
//   theme.value = 'light';
// }, { immediate: true })

// 始终设定为light模式
provide('isRealDark', false);
</script>

<template>
  <van-config-provider :theme="theme">
    <router-view />
  </van-config-provider>
</template>
