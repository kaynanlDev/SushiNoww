<script setup></script>

<template>
  <header>
    <div class="container flex justify-between items-center">
      <div class="logo">
        <img class="w-full" src="../assets/sushi.svg" alt="logo SushiNow" />
      </div>
      <nav class="flex items-center">
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
        <button
          class="bg-(--color-primary) text-sm duration-200 ease-in hover:opacity-75 hover:cursor-pointer py-2 px-8 rounded-3xl text-(#fff)"
        >
          Baixar o App
        </button>
      </nav>
    </div>
  </header>
</template>

<style scoped>
button {
  color: #fff;
}
</style>
