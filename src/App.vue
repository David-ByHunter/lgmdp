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
  --color-primary: #3D0000;
  --color-secondary: #954200;
  --color-accent: #F28E1C;
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
