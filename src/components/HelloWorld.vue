<script setup lang="ts">
import { ref } from 'vue';

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <section hello-world>
    <h1>{{ msg }}</h1>
  </section>
</template>

<style lang="postcss">
[hello-world] {
  @apply flex justify-center items-center;
  h1 {
    @apply text-3xl;
  }
}
</style>
