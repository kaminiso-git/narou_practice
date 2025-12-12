<template>
  <div :class="$style.container">
    <SideBarButton label="Apple" @click="fruit = 'Apple'" />
    <SideBarButton label="Banana" @click="fruit = 'Banana'" />
    <SideBarButton label="Orange" @click="fruit = 'Orange'"/>
    <SideBarButton label="Lemon" @click="fruit = 'Lemon'"/>
  </div>
</template>

<script setup lang="ts">
import SideBarButton from './SideBarButton.vue'
const fruit = defineModel<string>('fruit')
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
