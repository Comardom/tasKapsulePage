<script setup lang="ts">

import Capsule from "@/promotion/Capsule.vue";
</script>

<template>
  <div class="layout">
    <div class="square"></div>
    <div class="ellipse-container">
      <Capsule :width="150"/>
      <Capsule :width="240"/>
      <Capsule :width="215"/>
      <Capsule :width="340"/>
    </div>
  </div>

</template>

<style scoped>
/* 整体布局：左右排列 */
.layout {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 750px; /* 左右间距 */
  height: 100vh; /* 占满窗口高度 */

}

/* 左边正方形 */
.square {
  width: 335px;
  height: 610px;
  background-color: #4a90e2;
  opacity: 0.25;
  animation: floatSquare 15s ease-in-out infinite;
}
@keyframes floatSquare {
  0%   { transform: translate(0, 0); }
  25%  { transform: translate(-5px, -20px); } /* 左上 */
  50%  { transform: translate(0, -35px); }    /* 正上 */
  75%  { transform: translate(5px, -20px); }  /* 右上 */
  100% { transform: translate(0, 0); }
}

/* 右边容器：上下排列两个椭圆 */
.ellipse-container {
  display: flex;
  flex-direction: column;
  gap: 120px; /* 椭圆之间的间距 */
  align-items: flex-end; /* 让子元素在容器右侧对齐 */
}
</style>