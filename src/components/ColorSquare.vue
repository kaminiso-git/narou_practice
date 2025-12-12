<template>
  <div :class="$style.container"></div>
</template>

<script setup lang="ts">
defineProps<{
  color?: string
}>()
</script>

<style module>
.container {
  width: 200px;
  height: 200px;
  background-color: v-bind('color');
  border-radius: 8px;
}
</style>
