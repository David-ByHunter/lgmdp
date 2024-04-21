<script setup lang="ts">
const props = defineProps<{
  text: string
}>()
</script>

<template>
  <div
    class="flex justify-center border-2 border-accent min-w-8 w-64 p-2 transition hover:bg-accent hover:text-primary hover:scale-105"
  >
    <p class="uppercase text-center font-bold m-4">{{ props.text }}</p>
</div>
</template>
