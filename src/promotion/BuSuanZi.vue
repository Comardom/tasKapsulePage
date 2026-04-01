<template>
  <div>
    今日总访问量 <span id="busuanzi_today_pv">加载中...</span> 次
    今日总访客数 <span id="busuanzi_today_uv">加载中...</span> 人
    本站总访问量 <span id="busuanzi_site_pv">加载中...</span> 次
    本站总访客数 <span id="busuanzi_site_uv">加载中...</span> 人
    本页总阅读量 <span id="busuanzi_page_pv">加载中...</span> 次
    本页总访客数 <span id="busuanzi_page_uv">加载中...</span> 人
  </div>
</template>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const script = document.createElement('script')
  script.src = '//cdn.busuanzi.cc/busuanzi/3.6.9/busuanzi.min.js'
  script.defer = true
  document.body.appendChild(script)
})
</script>
