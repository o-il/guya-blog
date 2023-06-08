<template>
  <div class="divider" ref="deviderDom"></div>
</template>

<script setup lang="ts" props="width">
import { onMounted, ref } from "vue";
const props = withDefaults(defineProps<{ width?: string }>(), {
  width: "100%",
});
const { width } = props;
const deviderDom = ref();
onMounted(() => {
  deviderDom.value.style.width = width;
});
</script>

<style lang="scss" scoped>
.divider {
  height: 1px;
  // background-color: white;
  background-color: rgba(255, 255, 255, 0.14);
}
</style>
