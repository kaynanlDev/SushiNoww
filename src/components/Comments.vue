<script setup>
const CommentsCard = [
  {
    id: 1,
    person: new URL("../assets/person-1.png", import.meta.url).href,
    name: "Daniele Almeida",
    commentTxt: "Ótimo serviço! Encantada com a qualidade dos pratos.",
    stars: new URL("../assets/stars.svg", import.meta.url).href,
  },
  {
    id: 2,
    person: new URL("../assets/person-2.png", import.meta.url).href,
    name: "Ricardo França",
    commentTxt:
      "Não é apenas a comida excelente, o serviço torna a experiência especial.",
    stars: new URL("../assets/stars.svg", import.meta.url).href,
  },
];
</script>
<template>
  <div class="container flex items-center justify-center flex-col">
    <h2 class="text-5xl font-p1 text-center mt-30 mb-20">Comentários</h2>
    <div class="flex flex-col md:flex-row justify-center gap-6 max-w-3/4">
      <div
        class="w-3/3 md:w-120 flex justify-center flex-col rounded-2xl p-6 bg-(--color-dark-20)"
        v-for="comment in CommentsCard"
        :key="comment.key"
      >
        <div class="h-18 w-18 rounded-full">
          <img :src="comment.person" alt="foto de uma pessoa" />
        </div>
        <h3 class="font-p1 text-2xl mt-4">{{ comment.name }}</h3>
        <p class="font-s2 text-base mt-4 mb-7">
          {{ comment.commentTxt }}
        </p>
        <div><img :src="comment.stars" alt="" /></div>
      </div>
    </div>
  </div>
</template>
