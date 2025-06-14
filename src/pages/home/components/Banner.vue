<script setup lang="ts">
import { defineComponent } from 'vue'

</script>

<template>
    <div class="banner">
        <img src="/src/assets/banner.jpg" alt="Banner Image">
    </div>
</template>

<style scoped>
.banner {
    width: 100vw;
    height: auto;
}

.banner img {
    margin-top: 2vw;
    width: 75vw;
    height: auto;
    box-shadow: 0px 0px 50px 0.5vw rgba(0, 0, 0, 0.8);
    border-radius: 20px;
    transition: all 0.5s ease-in-out;
    transform: scale(1);
}

.banner img:hover {
    transform: scale(1.01);
    transition: all 0.5s ease-in-out;
}
</style>