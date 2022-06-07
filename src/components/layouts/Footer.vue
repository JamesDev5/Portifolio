<template>
  <footer >
    <div class="row bg-secondary mb-0 p-5">
      <div class="col-lg-6 col-sm-12 align-self-center text-center text-light">
        © 2022: Desenvolvido Por James Mendonça 
      </div>

      <div class="col-lg-6 col-sm-12 align-self-end text-center text-light">
        <h5>DEIXE UMA MENSAGEM!</h5>
        <ul>
          <li>
            <a href="https://wa.me/5567991642807" target="_blank">
              <i class="fa-brands fa-whatsapp"></i> WhatsApp: (67) 9
              9164-2807</a
            >
          </li>

          <li>
            <a
              href="https://www.instagram.com/jamesmendoncajr/"
              target="_blank"
            >
              <i class="fa-brands fa-instagram"></i> Instagram: James Mendonça
              Jr</a
            >
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
body {
  width: 100%;
  height: 10px;
  font-weight: bold;
}
li {
  list-style: none;
}
a {
  font-size: 18px;
  color: white;
  text-decoration: none;
}

a:visited {
  color: white;
  text-decoration: none;
}
</style>
