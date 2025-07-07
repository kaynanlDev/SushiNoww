<script setup>
import Button from "./Button.vue";
import { ref } from "vue";
let menuMobile = ref(false);
</script>

<template>
  <header>
    <div class="container flex justify-between items-center">
      <div class="logo">
        <img class="w-full" src="../assets/sushi.svg" alt="logo SushiNow" />
      </div>
      <nav class="hidden md:flex items-center">
        <ul class="flex gap-6 mr-9">
          <li>
            <a class="text-sm duration-200 ease-in hover:opacity-75" href="#"
              >Início</a
            >
          </li>
          <li>
            <a class="text-sm duration-200 ease-in hover:opacity-75" href="#"
              >Sobre nós</a
            >
          </li>
          <li>
            <a class="text-sm duration-200 ease-in hover:opacity-75" href="#"
              >Populares</a
            >
          </li>
        </ul>
        <Button btnText="Baixar o App" />
      </nav>
      <div
        v-if="menuMobile === false"
        class="md:hidden cursor-pointer"
        @click="menuMobile = true"
      >
        <img src="../assets/hamburguer.svg" alt="icon menu-hamburger" />
      </div>
    </div>
    <div
      v-if="menuMobile === true"
      class="absolute top-0 right-0 p-4 flex flex-col md:hidden w-3/5 h-full bg-(--color-dark-20)"
    >
      <div
        class="justify-items-end mb-8 cursor-pointer"
        @click="menuMobile = false"
      >
        <img src="../assets/close.svg" alt="icon close" />
      </div>
      <nav class="flex flex-col items-center">
        <ul class="flex items-center justify-center gap-6 mb-9 flex-col">
          <li>
            <a class="text-base duration-200 ease-in hover:opacity-75" href="#"
              >Início</a
            >
          </li>
          <li>
            <a class="text-base duration-200 ease-in hover:opacity-75" href="#"
              >Sobre nós</a
            >
          </li>
          <li>
            <a class="text-base duration-200 ease-in hover:opacity-75" href="#"
              >Populares</a
            >
          </li>
        </ul>
        <Button btnText="Baixar o App" />
      </nav>
    </div>
  </header>
</template>

<style scoped>
button {
  color: #fff;
}
header {
  font-family: "poppins", sans-serif;
}
</style>
