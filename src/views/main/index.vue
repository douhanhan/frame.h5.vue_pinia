<script setup lang="ts">
import { ref, reactive } from 'vue';
import axios from "axios";
import dayjs from "dayjs";
import classNames from "classnames";

const loading = ref(true);
const finished = ref(false);
let list = reactive([]);

const onLoad = () => {
  loading.value = true;
}

onMounted(() => onLoad())

</script>

<template>
  <div class="rank-container">
    <van-row>
       这里是空白区间
      </van-row>
  </div>
</template>

<style lang="less" scoped>
.rank-container {
  padding: 0px;
  color: #333333;
}
</style>