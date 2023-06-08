<template>
  <div class="homeWarp">
    <!-- 背景图片 -->
    <img class="background" :src="imgList[2]" alt="" />
    <div class="overviewWarp">
      <!-- 个人信息组件 -->
      <PersonalOverview class="overview" />
      <!-- 按钮组 -->
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import bg01 from "@/assets/img/bg_01.jpg";
import PersonalOverview from "@/components/biz/personal/PersonalOverview.vue";

const imgList = ref([
  "https://pic3.zhimg.com/v2-3b83e03ec8352b504e7a3dab903a9c66_r.jpg",
  "https://cdn.pixabay.com/photo/2017/08/05/22/09/island-2586047_1280.jpg",
  bg01,
]);
</script>

<style lang="scss" scoped>
.homeWarp {
  position: relative;
  height: 100vh;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  .background {
    z-index: -1;
    position: absolute;
    width: 100%;
  }

  .overviewWarp {
    .overview {
    }
  }
}
</style>
