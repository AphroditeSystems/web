<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Sidebar from './components/Sidebar.vue'
</script>

<template>
  <div class="flex">
    <div class="flex-shrink-0">
      <Sidebar />
    </div>
    <RouterView />
  </div>
</template>
