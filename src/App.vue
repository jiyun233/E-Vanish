<script setup lang="ts">
import { RouterView } from "vue-router";
import Loading from "./animation/Loading.vue";
import { ref } from "vue";
</script>

<template>
  <Loading />
  <RouterView />
</template>

<style scoped>
section {
  height: 100vh;
  overflow: auto;
}
</style>
