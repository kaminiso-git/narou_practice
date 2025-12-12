<script setup lang="ts">
import MainContent from './components/MainContent.vue'
import SideBar from './components/SideBar.vue'
</script>

<template>
  <div :class="$style.container">
    <SideBar />
    <MainContent />
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
