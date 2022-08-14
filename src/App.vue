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
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  font-weight: 300;
}

@media (max-width: 600px) {
  body {
    font-size: 14px;
  }
}

h1,
h2,
h3,
h4,
h5,
h6 {
  margin: 0;
  padding: 0;
  font-weight: 600;
}

h1 {
  font-size: 2.5em;
  text-align: center;
  margin: 1em 0;
}

h2 {
  font-size: 1.6em;
}

p {
  margin: 0 0 1.4em 0;
}

main {
  padding: 0 10% 2% 10%;
}

p img {
  max-width: 100%;
}
</style>
