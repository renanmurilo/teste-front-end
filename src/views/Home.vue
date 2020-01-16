<template>
  <div class="home">
    <Banner />
    <Conteudo />
  </div>
</template>

<script>
import Banner from "@/components/Banner.vue";
import Conteudo from "@/components/Conteudo.vue";

export default {
  components: {
    Banner, 
    Conteudo
  },
  created() {
    document.title = "Dev";
  }
};
</script>
