<template>
  <div :class="$style.container">
    <div :class="$style.title">Title</div>
    <div>{{ `${fruit} `.repeat(40).trim() }}</div>
    <div :class="$style.squares">
      <ColorSquare color="red" />
      <ColorSquare color="lime" />
      <ColorSquare color="blue" />
    </div>
  </div>
</template>

<script setup lang="ts">
import ColorSquare from './ColorSquare.vue'

defineProps<{
  fruit: string
}>()
</script>

<style module>
.container {
  border: 1px solid red;
  width: 1000px;
  margin: auto;
  height: 100%;
  padding-top: 200px;
}

.title {
  font-size: 40px;
}

.squares {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
</style>
