<!-- src/animation/Loading.vue -->
<script setup lang="ts">
import { ref, onMounted } from "vue";

const show = ref(false);
const backgroundOpacity = ref(1);

onMounted(() => {
    setTimeout(() => {
        show.value = true;
    }, 0);

    setTimeout(() => {
        show.value = false;
    }, 3000);

    setTimeout(() => {
        backgroundOpacity.value = 0;
    }, 2500);
});
</script>

<template>
    <div class="overlay" :style="{ opacity: backgroundOpacity }">
        <div class="logo-container">
            <Transition name="fade">
                <img v-if="show" src="/logo.png" alt="logo" class="responsive-logo" />
            </Transition>
        </div>
    </div>
</template>

<style>
.overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #f0f0f0;
    z-index: 1000;
    display: flex;
    justify-content: center;
    align-items: center;
    pointer-events: none;
    transition: opacity 3s ease;
}

.logo-container {
    display: flex;
    justify-content: center;
    align-items: center;
}

.responsive-logo {
    width: min(35vw, 1080px);
    height: auto;
}

.fade-enter-active,
.fade-leave-active {
    transition: opacity 3s ease;
}

.fade-enter-from,
.fade-leave-to {
    opacity: 0;
}

.fade-enter-to,
.fade-leave-from {
    opacity: 1;
}
</style>
