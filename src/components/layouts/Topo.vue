<template>
  <div class="content">
    <nav class="navbar navbar navbar-light  bg-secondary navbar-expand-lg" style="--bs-bg-opacity:.5">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Portifólio</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a
                class="nav-link "
                aria-current="page"
                href="#"
                @click="navegarPara('Home')"
                >Home</a
              >
            </li>
            <li class="nav-item">
              <a
                class="nav-link "
                href="#"
                aria-current="page"
                @click="navegarPara('Projects')"
                >Projetos</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#" @click="navegarPara('About')"
                >Sobre</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Topo",
  methods: {
    navegarPara(p) {
      this.$emit("navegar", p);
    },
  },
};
</script>
<style scoped>

</style>

