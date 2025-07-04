<script setup>
const popularFood = [
  {
    id: 1,
    name: "Ramem de frango",
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    price: "30",
    image: new URL("../assets/ramem-frango.png", import.meta.url).href,
  },
  {
    id: 2,
    name: "Ramem apimentado",
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    price: "30",
    image: new URL("../assets/ramem-apimentado.png", import.meta.url).href,
  },
  {
    id: 3,
    name: "Ramem tradicional",
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    price: "30",
    image: new URL("../assets/ramem-tradicional.png", import.meta.url).href,
  },
];
</script>
<template>
  <div class="container">
    <h2 class="text-5xl font-p1 text-center mb-27 mt-30">Populares</h2>
    <div class="grid grid-cols-3 gap-6 justify-center">
      <div
        class="flex items-center justify-center flex-col bg-(--color-dark-20) rounded-2xl p-6"
        v-for="food in popularFood"
        :key="food.id"
      >
        <img
          class="w-[70%] mt-[-5rem]"
          :src="food.image"
          alt="comida popular"
        />
        <h3 class="font-p1 text-2xl mt-4">{{ food.name }}</h3>
        <p class="text-center font-s2 text-base py-6">{{ food.description }}</p>
        <p class="price font-p1 text-xl">R${{ food.price }}</p>
      </div>
    </div>
  </div>
</template>
<style>
.price {
  color: #ff0000;
}
</style>
