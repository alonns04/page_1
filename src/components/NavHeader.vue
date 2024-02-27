<script setup>
</script>


<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-8">
        <div class="row" style="margin-top: 10px; margin-bottom: 10px;">
          <div class="col-4">
            <nav class="navbar navbar-expand-md bg-body-tertiary">
              <div class="container-fluid">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                  data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                  aria-label="Toggle navigation">
                  <span class="navbar-toggler-icon navbar-dark"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                  <div class="navbar-nav">
                    <a class="nav-link options" href="#">Inicio</a>
                    <a class="nav-link options" href="#">Nosotros</a>
                    <a class="nav-link options" href="#">Contáctanos</a>
                  </div>
                </div>
              </div>
            </nav>
          </div>
        </div>

      </div>
      <div class="col-4">

        <div class="row">
          <ul class="nav col-12 justify-content-end" style="align-items: center;">
            <li class="ms-3"><a href="">
                <img id="navimage" height="80" style=""
                  src="https://www.creativefabrica.com/wp-content/uploads/2021/03/20/Mountain-logo-Design-Graphics-9785421-1-580x435.png"
                  alt="">
              </a>
            </li>
          </ul>
        </div>

      </div>
    </div>
  </div>
</template>


<style scoped>
.nameBrand {
  font-family: fantasy;
  text-align: left;
}

nav {
  background-color: rgb(0, 0, 0) !important;
}

a {
  color: white !important;
}

div {
  color: white;
  background-color: black;
}

p {
  margin-top: 8px !important;
  margin-right: 46px !important;
}

.options{
  border-radius: 100px;
}
.options:hover {
      background-color: antiquewhite;
      color: black !important;
}

#navimage:hover{
  animation: sacudir 0.5s ease 1;
}




@keyframes sacudir {
      0% { transform: translateX(0); }
      25% { transform: translateX(-3px) rotate(-3deg); }
      50% { transform: translateX(3px) rotate(3deg); }
      75% { transform: translateX(-3px) rotate(-3deg); }
      100% { transform: translateX(0); }
    }


</style>