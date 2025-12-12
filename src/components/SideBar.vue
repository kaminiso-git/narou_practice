<template>
  <div :class="$style.container">
    <SideBarButton /><SideBarButton /><SideBarButton /><SideBarButton />
  </div>
</template>

<script setup lang="ts">
import SideBarButton from './SideBarButton.vue'
</script>

<style module>
.container {
  background-color: rgb(228, 228, 228);
  width: 400px;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
