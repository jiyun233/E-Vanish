<script setup lang="ts">
import { defineComponent } from 'vue'
import { NDivider, NCard, NButton } from 'naive-ui'
import Banner from './components/Banner.vue'
import NewsCard from './components/NewsCard.vue'
import Background from '../Background.vue'
import '/vfonts/FiraCode.css'

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
    width: 75vw;
    height: 100vw;
    margin: auto;
}

.divider {
    width: 75vw;
}
</style>
