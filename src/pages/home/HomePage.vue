<script setup lang="ts">
import { defineComponent } from 'vue'
import { NDivider, NCard, NButton } from 'naive-ui'
import Banner from './components/Banner.vue'
import NewsCard from './components/NewsCard.vue'
import Background from '../Background.vue'

</script>

<template>
    <div class="home-page">
        <Banner />
        <br />
        <n-divider dashed class="divider" />
        <br />
        <NewsCard />
    </div>
    <Background />
</template>

<style scoped>
.home-page {
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    /* 水平居中 */
    align-items: center;
    /* 垂直顶部对齐 */
    margin: auto;
    flex-direction: column;
    /* 垂直堆叠子元素 */
    /* overflow: hidden; */

}

.divider {
    width: 75vw;
}
</style>
