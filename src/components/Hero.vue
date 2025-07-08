<script setup>
import Button from "./Button.vue";
</script>
<template>
  <div class="container grid grid-cols-1 md:grid-cols-2 h-screen">
    <div
      class="hero-text flex flex-col items-center md:items-start md:justify-center mb-12"
    >
      <h1 class="text-5xl font-p1">Comida Oriental</h1>
      <p
        class="font-s2 text-base text-center md:text-start max-w-3/4 mt-[18px] mb-12"
      >
        A culinária Japonesa é bastante equilibrada, sendo muito rica em peixes
        (ômega 3), vegetais, massas e ingredientes frescos.
      </p>
      <Button class="max-w-3xs py-3 font-s2" btnText="Ver o cardápio" />
    </div>
    <div class="hero-img flex items-center justify-center">
      <img
        class="w-[60%] lg:w-3/5 h-full"
        src="../assets/sushi-hero.png"
        alt="sushi hero"
      />
    </div>
  </div>
</template>
<style scoped>
button {
  color: #fff;
}
</style>
