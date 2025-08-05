<template>
  <a target="_blank" :href="link" class="link"
    ><button>
      <img v-bind:src="imgSrc" class="icon" />{{ name }}
    </button></a
  >
</template>

<script setup lang="ts">
const props = defineProps<{
    link: string;
    imgSrc: string;
    name: string;
}>();
</script>

<style>
.icon {
  height: 0.8em;
  margin-right: 0.5em;
}

.link:hover {
  border-width: 0;
  filter: drop-shadow(0 0 1em #ffffff);
}
</style>