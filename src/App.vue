<template>
  <Topo @navegar="componente = $event" />
  <Conteudo v-if="visibilidade" :conteudo="componente"/>

  <Footer />
</template>

<script>
import Conteudo from "./components/layouts/Conteudo.vue";
import Topo from "./components/layouts/Topo.vue";
import Footer from "./components/layouts/Footer.vue";

export default {
  name: "App",
  data: () => ({
    visibilidade: true,
    componente: "Home",
  }),
  components: {
    Topo,
    Conteudo,
    Footer,
  },
};
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap');

body{
  overflow-x: hidden;
  background-color: white;
  
}
</style>
