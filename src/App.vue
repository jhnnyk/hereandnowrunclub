<script setup>
import { RouterLink, RouterView } from 'vue-router';
import NavBar from './components/NavBar.vue';
</script>

<template>
  <NavBar />

  <RouterView />
</template>

<style>
body {
  margin: 0;
  padding: 0;
  font-family: 'Quicksand', sans-serif;
}

main {
  padding: 2% 10%;
}
</style>
