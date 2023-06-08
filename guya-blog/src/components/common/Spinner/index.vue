<template>
  <div v-if="loading" class="loading">this is loading animation</div>
</template>

<script setup lang="ts" props="loading">
defineProps<{ loading: boolean }>();
</script>

<style lang="scss" scoped>
.loading {
  width: 100%;
  height: 100%;
  background: white;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 999;
}
</style>
