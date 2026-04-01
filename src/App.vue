<script setup lang="ts">
import Literary from "@/promotion/Literary.vue";
import SchemaPic from "@/promotion/SchemaPic.vue";
import BuSuanZi from "@/promotion/BuSuanZi.vue";
import Footer from "@/promotion/CopyrightFooter.vue";
</script>

<template>
  <div class="page-container">
    <Literary />
    <Schema-pic />
    <BuSuanZi />
    <Footer
      year="2026"
      owner="Comardom"
      email="Comardom@outlook.com"
      icpNumber="辽ICP备2025060502号-2"
      policeNumber="辽公网安备21021702000880号"
      policeLink="https://www.beian.gov.cn/portal/registerSystemInfo?recordcode=21021702000880"
  />
  </div>
</template>

<style scoped>
.page-container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  background: repeating-linear-gradient(
      to right,
      #f0f0f0,
      #f0f0f0 2px,
      #ffffff 1px,
      #ffffff 4px
  );
  min-height: 98.4vh;
}
</style>
