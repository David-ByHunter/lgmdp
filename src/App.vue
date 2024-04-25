<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <main>
    <RouterView />
  </main>
</template>

<style>
:root {
  --color-primary: rgb(61,0,0);
  --color-secondary: rgb(194,55,5);
  --color-accent: rgb(245,198,67);
}
body {
  display: flex;
  height: 100vh;
  width: 100%;
}
#app {
  height: inherit;
  width: inherit;
  background-color: var(--color-primary);
  color: var(--color-accent);
}
</style>
