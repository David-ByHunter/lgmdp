<script setup lang="ts">
import githubIcon from '@/assets/githubIcon.vue'
import instagramIcon from '@/assets/instagramIcon.vue'
import { socialMedia } from '@/components/data/links.ts'
</script>

<template>
  <div class="flex justify-center gap-x-8 text-accent *:size-8">
    <a
      class="hover:scale-110"
      :href="socialMedia[0].link"
      :alt="socialMedia[0].alt"
      target="_blank"
      :aria-label="socialMedia[0].title"
    >
      <githubIcon />
    </a>
    <a
      class="hover:scale-110"
      :href="socialMedia[1].link"
      :alt="socialMedia[1].alt"
      target="_blank"
      :aria-label="socialMedia[1].title"
    > 
      <instagramIcon />
    </a>
  </div>
</template>
