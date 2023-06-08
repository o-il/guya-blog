<template>
  <div class="personalOverview">
    <!-- 头像 -->
    <div class="avatarWarp">
      <img class="avatar" :src="avatar" alt="" />
    </div>
    <!-- 名称 -->
    <div class="name">谷芽</div>
    <!-- 分割线 -->
    <Divider class="divider" width="310px" />
    <!-- 个性签名 -->
    <div class="signature">一代人终将老去，但总有人正年轻</div>
  </div>
</template>

<script setup lang="ts">
import avatar from "@/assets/img/avatar.png";
import Divider from "@/components/common/Divider/index.vue";
</script>

<style lang="scss" scoped>
.personalOverview {
  width: 100%;
  display: flex;
  flex-direction: column;
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
      bottom: -3px;
      width: 100%;
    }
  }
  .name {
    font-size: 30px;
    margin: 5px 0 0 0;
    color: white;
  }
  .signature {
    font-size: 12px;
    color: white;
  }
  .divider {
    margin: 20px 0;
  }
}
</style>
