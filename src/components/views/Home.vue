<template>
  <div class="container-fluid">
    <div class="row  justify-content-center py-5">
      <div class="col-lg-12 col-sm-12 text-center ">
        <Efeito />
      </div>

    <div class="row justify-content-evenly py-5">
      <a
        class="col-lg-3 col-sm-6 m-4 text-center btn"
        href="https://github.com/JamesDev5"
        target="_blank"
      >
        <div class="fa-brands fa-github">GitHub</div>
      </a>
      
      <a
        class="col-lg-3 col-sm-6  m-4 text-center btn"
        href="https://www.linkedin.com/in/james-c-mendon%C3%A7a-jr-2483aa1b9/"
        target="_blank"
      >
        <div class="fa-brands fa-linkedin">Linkedin</div>
      </a>
    </div>
  </div>
    </div>

</template>

<script>
import Efeito from "@/components/others/Efeito.vue";
export default {
  name: "Home",
  components: {
    Efeito,
  },
};
</script>

<style scoped >
.btn {
  font-size: 24px;
  color: white;
  background-color: rgb(34, 59, 59);
  height: 50px;
  border: 2px solid #ec710c;
  transition: 0.8s;
  letter-spacing: 0.5cm;
  font-weight: 700;
}
.btn:hover {
  color: #16408d;
  background-color: transparent;
  height: 50px;
  border: 2px solid #000;
  transition: 0.8s;
}
.btn a {
  text-decoration: none;
  transition: 0.8s;
}

</style>