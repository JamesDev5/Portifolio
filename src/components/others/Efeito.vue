<template >
  <h1>{{ texto }}</h1>
</template>

<script>
export default {
  name: "Efeito",
  data: () => ({
    texto: "JAMES MENDONÇA  -  DESENVOLVEDOR FRONT-END",
  }),
  activated() {
    const textoArray = this.texto.split("");
    this.texto = "";
    textoArray.forEach((letra, indice) => {
      setTimeout(() => (this.texto += letra), 50*indice);
    });
  },
};
</script>

<style scoped>
h1 {
  font-family: "Roboto", Courier, monospace;
  font-weight: 800;
  color: black;
  text-shadow: 1px 1px white;
}
h1::after {
  content: "|";
  margin-left: 5px;
  opacity: 1;
  animation: piscar 0.7s infinite;
}
@keyframes piscar {
  0%,
  100% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
}
</style>