<script setup>
import NavFooter from "./NavFooter.vue";
</script>
<template>
  <NavFooter />

  <div
    class="container flex flex-col items-center sm:flex-row gap-6 sm:gap-0 justify-between"
  >
    <div class="logo">
      <img src="../assets/sushi.svg" alt="logo do Sushinow" />
    </div>
    <nav class="flex gap-2">
      <a
        class="h-8 w-8 p-1 rounded-full flex items-center justify-center border-1 border-(--color-dark-10)"
        href="#"
      >
        <img src="../assets/FacebookLogo.svg" alt="logo do Facebook"
      /></a>
      <a
        href="#"
        class="h-8 w-8 p-1 rounded-full flex items-center justify-center border-1 border-(--color-dark-10)"
        ><img src="../assets/InstagramLogo.svg" alt="logo do Instagram"
      /></a>
      <a
        href="#"
        class="h-8 w-8 p-1 rounded-full flex items-center justify-center border-1 border-(--color-dark-10)"
        ><img src="../assets/TwitterLogo.svg" alt="logo do Twitter"
      /></a>
    </nav>
  </div>
</template>

<style scoped>
a {
  transition: 0.3s ease-in-out;
}
a:hover {
  opacity: 0.8;
}
</style>
