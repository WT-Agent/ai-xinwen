<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了科技公司 A 轮融资新闻通稿撰写"
  },
  {
    "text": "用户 189****7744 得到了新品发布会倒金字塔规范新闻稿"
  },
  {
    "text": "用户 131****3399 完成了企业公益慈善捐赠社会责任新闻稿"
  },
  {
    "text": "用户 156****4400 生成了针对网传误会的企业诚恳公关声明"
  },
  {
    "text": "用户 173****8855 取得了主流科技媒体发稿与 SEO 优化 SOP"
  }
]);
</script>
