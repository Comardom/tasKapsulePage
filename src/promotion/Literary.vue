<script setup lang="ts">

</script>

<template>
  <div class="literary-piece">
    <h1>TasKapsule胶囊任务助手</h1>
    <hr />
    <h2>敬请期待</h2>
    <p>镁光在身后膨胀坠落<br />
      记得比耶哦<br />
      下次便是他冬另朵</p>
  </div>
</template>

<style scoped>
.literary-piece {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  //margin: auto;
  position: absolute;   /* 绝对定位 */
  top: 50%;             /* 距离顶部 50% */
  left: 50%;            /* 距离左侧 50% */
  transform: translate(-50%, -50%); /* 往回偏移自身宽高的一半 */
  text-align: center;   /* 文本居中 */
}

.literary-piece h1 {
  font-size: 3rem;   /* 主标题更大 */
}

.literary-piece h2 {
  font-size: 2rem;   /* 副标题稍小 */
}

.literary-piece p {
  font-size: 1.2rem; /* 正文比默认大一点 */
  line-height: 1.8;  /* 行距加宽，阅读更舒服 */
}
</style>