<template>
  <div class="homeWarp">
    <!-- 背景图片 -->
    <img class="background" :src="imgList[0]" alt="" />
    <div class="overviewWarp">
      <!-- 个人信息组件 -->
      <PersonalOverview class="overview" />
      <!-- 按钮组 -->
    </div>
  </div>
</template>

<script setup lang="ts">
// https://www.iculture.cc/demo/intro/1/#
// https://blog.zhlzzz.com/
import { ref } from "vue";
import bg01 from "@/assets/img/bg_01.jpg";
import bg02 from "@/assets/img/bg_02.jpg";
import bg03 from "@/assets/img/bg_03.jpg";
import bg04 from "@/assets/img/bg_04.jpg";
import bg05 from "@/assets/img/bg_05.jpg";
import PersonalOverview from "@/components/biz/personal/PersonalOverview.vue";

const imgList = ref([
  "https://pic3.zhimg.com/v2-3b83e03ec8352b504e7a3dab903a9c66_r.jpg",
  bg01,
  bg02,
  bg03,
  bg04,
  bg05,
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
    height: 100%;
    object-fit: cover; /* 图片填满容器,可能裁剪 */
  }

  .overviewWarp {
    .overview {
    }
  }
}
</style>
