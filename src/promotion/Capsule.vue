<script setup lang="ts">
// import { defineProps } from 'vue'

// 定义一个宽度参数，默认值 200px
const props = defineProps<{
  width?: string | number
}>()
</script>

<template>
  <div class="ellipse" :style="{ width: typeof width === 'number' ? width + 'px' : width }"></div>
</template>

<style scoped>
/* 跑道形状椭圆（胶囊形） */
.ellipse {
  height: 80px;
  background-color: #e94e77;
  opacity: 0.25;
  border-radius: 40px; /* 高度的一半，形成跑道形状 */
  animation: floatCapsule 10s ease-in-out infinite;
}
.ellipse:nth-child(1) { animation-duration: 8s;animation-delay: 13s; }
.ellipse:nth-child(2) { animation-duration: 10s; animation-delay: 11s; }
.ellipse:nth-child(3) { animation-duration: 15s; animation-delay: 7s; }
.ellipse:nth-child(4) { animation-duration: 20s; animation-delay: 5s; }

@keyframes floatCapsule {
  0%   { transform: translateX(0); }
  50%  { transform: translateX(20px); } /* 向右轻微漂移 */
  100% { transform: translateX(0); }
}
</style>