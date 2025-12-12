<template>
  <div :class="$style.container">
    <div>{{ label }}</div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  label: string
}>()
</script>

<style module>
.container {
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 20px;
}
</style>
