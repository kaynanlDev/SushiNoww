<script setup>
import { defineProps } from "vue";

defineProps({
  btnText: String,
});
</script>

<template>
  <button
    class="bg-(--color-primary) text-sm duration-300 ease-in-out hover:opacity-75 hover:cursor-pointer py-2 px-8 rounded-3xl"
  >
    {{ btnText }}
  </button>
</template>
