<template>
  <div class="app-container">
    <!-- 基础用法 -->
    <TextScroll text="这是一条基础的滚动公告，默认向左滚动。" typewriter />

    <!-- 使用不同的类型 -->
    <TextScroll type="success" text="这是一条成功类型的滚动公告" typewriter />

    <TextScroll type="warning" text="这是一条警告类型的滚动公告" />

    <TextScroll type="danger" text="这是一条危险类型的滚动公告" />

    <TextScroll type="info" text="这是一条信息类型的滚动公告" />

    <!-- 自定义速度和方向 -->
    <TextScroll text="这是一条速度较慢、向右滚动的公告" :speed="30" direction="right" show-close />
  </div>
</template>

<script setup lang="ts">
import TextScroll from "@/components/TextScroll/index.vue";
</script>

<style lang="scss" scoped>
.app-container {
  :deep(.text-scroll-container) {
    margin-bottom: 20px;
  }
}
</style>
