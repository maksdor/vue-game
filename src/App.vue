<script setup>

import Header from './components/Header.vue';
import GameCard from './components/GameCard.vue';
import { RouterView } from "vue-router";

</script>

<template>
  <div class = 'app'>
    <Header/>
    <RouterView/>
  </div>
</template>

<style scoped>
.app {
  width: 100%;
  min-height: 100vh;
  background: #343B3F;
}
</style>
