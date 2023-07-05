<script setup>
import { RouterView } from 'vue-router'
import TodoHeader from './components/TodoHeader.vue';
</script>

<template>
  <TodoHeader />
  <RouterView />
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&display=swap');

*{
  font-family: "Poppins", sans-serif;
}
body{
  background: url(assets/homepic.png), lightgray 50% / cover no-repeat;
  background-size: 100%;
}
@media (max-width: 768px) {
  body {
  background: url(assets/homepic-resized.png), lightgray 50% / cover;
  background-size: 100%;
  background-repeat: no-repeat;
  }
}
</style>
