<template>
  <div class="homeWarp">
    <!-- 背景图片 -->
    <img class="background" :src="imgList[2]" alt="" />
    <!-- 个人信息组件 -->
    <!-- 按钮组 -->
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import bg01 from "@/assets/img/bg_01.jpg";

const imgList = ref([
  "https://pic3.zhimg.com/v2-3b83e03ec8352b504e7a3dab903a9c66_r.jpg",
  "https://cdn.pixabay.com/photo/2017/08/05/22/09/island-2586047_1280.jpg",
  bg01,
]);
</script>

<style lang="scss" scoped>
.homeWarp {
  height: 100vh;
  overflow: hidden;
  .background {
    width: 100%;
  }
}
</style>
