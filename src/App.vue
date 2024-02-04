<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import TopNav from './components/TopNav.vue';
import BottomNav from './components/BottomNav.vue';
</script>

<template>
  <TopNav />
  <RouterView />
  <BottomNav />
</template>
