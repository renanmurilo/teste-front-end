<template>
  <div>
    <Banner />
    <Conteudo />
  </div>
</template>

<script>
import Banner from "@/components/Banner.vue";
import Conteudo from "@/components/Conteudo.vue";

export default {
  name: "home",
  components: {
    Banner, 
    Conteudo
  },
  created() {
    document.title = "Dev";
  }
};
</script>
