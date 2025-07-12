<script setup></script>
<template>
  <div
    class="container flex justify-center border-b-1 border-b-(--color-dark-20)"
  >
    <div class="w-3/4 flex md:flex-row justify-between">
      <nav class="mt-6 md:mt-30">
        <ul>
          <h4 class="text-base mb-1">Produto</h4>
          <li><a href="#">Todos</a></li>
          <li><a href="#">Sushi</a></li>
          <li><a href="#">Premium</a></li>
        </ul>
      </nav>
      <nav class="mt-6 md:mt-30">
        <ul>
          <h4 class="text-base mb-1">Informações</h4>
          <li><a href="#">FAQ</a></li>
          <li><a href="#">Blog</a></li>
          <li><a href="#">Suporte</a></li>
        </ul>
      </nav>
      <nav class="mt-6 md:mt-30 hidden md:block">
        <ul>
          <h4 class="text-base mb-1">Empresa</h4>
          <li><a href="#">Sobre nós</a></li>
          <li><a href="#">Local</a></li>
          <li><a href="#">Contato</a></li>
        </ul>
      </nav>
      <nav class="mt-6 md:mt-30 hidden md:block">
        <ul>
          <h4 class="text-base mb-1">Social</h4>
          <li><a href="#">Facebook</a></li>
          <li><a href="#">Instagram</a></li>
          <li><a href="#">Twitter</a></li>
        </ul>
      </nav>
    </div>
  </div>
</template>
<style scoped>
h4 {
  font-family: "Koh Santepheap", serif;
}
a {
  font-family: "poppins", sans-serif;
  font-size: 14px;
  transition: 0.3s ease-in-out;
  padding: 4px 0;
}
a:hover {
  opacity: 0.8;
}
</style>
