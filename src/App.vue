<script setup>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import About from "./components/About.vue";
import Popular from "./components/Popular.vue";
import Comments from "./components/Comments.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <Header />
  <main>
    <Hero />
    <About />
    <Popular />
    <Comments />
  </main>
  <Footer />
  <p class="w-full text-xs text-center pb-1">
    &copy;Todos os direitos reservados -
    <a
      class="hover:underline"
      target="_blank"
      href="https://github.com/kaynanlDev"
      >KaynanDev</a
    >
  </p>
</template>
