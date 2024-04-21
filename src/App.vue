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
  color: var(--color-accent);
  background-color: rgba(61,0,0,0.9);
}
#app::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('/BgImageKegs.webp');
  background-size: cover;
  z-index: -1;
}
</style>
