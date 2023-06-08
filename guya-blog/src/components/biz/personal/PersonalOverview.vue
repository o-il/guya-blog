<template>
  <div class="personalOverview">
    <!-- 头像 -->
    <div class="avatarWarp">
      <img class="avatar" :src="avatar" alt="" />
    </div>
    <!-- 名称 -->
    <!-- 个性签名 -->
  </div>
</template>

<script setup lang="ts">
import avatar from "@/assets/img/avatar.png";
</script>

<style lang="scss" scoped>
.personalOverview {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  .avatarWarp {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    overflow: hidden;
    position: relative;
    .avatar {
      position: absolute;
      bottom: 0px;
      width: 100%;
    }
  }
}
</style>
