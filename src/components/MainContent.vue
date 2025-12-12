<template>
  <div :class="$style.container">
    <div :class="$style.title">Title</div>
    <div>{{ 'Apple '.repeat(40).trim() }}</div>
  </div>
</template>

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
</style>
