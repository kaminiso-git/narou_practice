<script setup lang="ts">
import { ref } from 'vue'
import MainContent from './components/MainContent.vue'
import SideBar from './components/SideBar.vue'
const fruit = ref('Apple')
</script>

<template>
  <div :class="$style.container">
    <SideBar v-model:fruit="fruit" />
    <MainContent :fruit="fruit" />
  </div>
</template>

<style module>
.container {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: row;
}
</style>
