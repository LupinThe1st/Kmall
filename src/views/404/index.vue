<template>
  <img style="width: 666px;" src="../../assets/images/error_images/404.png" alt="" />
  <el-button
    @click="goHome"
    style="position: absolute; top: 0; left: 0; margin: 10px"
    type="primary"
  >
    首页
  </el-button>
</template>

<script setup lang="ts">
import { useRouter } from 'vue-router'
let $router = useRouter()
const goHome = () => {
  $router.push('/home')
}
</script>

<style scoped lang="scss">
img {
  display: block;
  margin: 0 auto;
}
</style>
