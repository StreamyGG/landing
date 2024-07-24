<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/blocks/Header.vue'
</script>

<template>
  <header>
   <Header />
  </header>

  <RouterView />
</template>
