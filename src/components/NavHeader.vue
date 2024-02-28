<script setup>
</script>


<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-6">
        <div class="row" style="margin-top: 10px; margin-bottom: 10px;">
          <div class="col-4">
            <nav class="navbar navbar-expand-md bg-body-tertiary">
              <div class="container-fluid">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
                  data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false"
                  aria-label="Toggle navigation">
                  <span class="navbar-toggler-icon navbar-dark"></span>
                </button>
                <div class="collapse navbar-collapse " id="navbarNavAltMarkup">
                  <div class="navbar-nav">
                    <a class="nav-link options" href="#">Inicio</a>
                    <a class="nav-link options" href="#">Nosotros</a>
                    <a class="nav-link options" href="#">Contáctanos</a>
                  </div>
                  <ul style="padding-top: 25px;" class="nav justify-content-around d-block d-sm-none">
                    <li class="ms-3"><a href=""><i class="bi bi-whatsapp" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-facebook" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-twitter" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-telegram" style="color: white;"></i></a></li>
                  </ul>
                </div>
              </div>
            </nav>
          </div>
        </div>

      </div>

      <div class="col-6">

        <div class="row justify-content-center ccc">
          <div class="col-1 d-none d-sm-block"></div>
          <div class="col-7 col-xs-4 d-none d-sm-block">
            <ul style="padding-top: 25px;" class="nav justify-content-around">
              <li class="ms-3"><a href=""><i class="bi bi-whatsapp" style="color: white;"></i></a></li>
              <li class="ms-3"><a href=""><i class="bi bi-facebook" style="color: white;"></i></a></li>
              <li class="ms-3"><a href=""><i class="bi bi-twitter" style="color: white;"></i></a></li>
              <li class="ms-3"><a href=""><i class="bi bi-telegram" style="color: white;"></i></a></li>
            </ul>

          </div>
          <div class="col-4 justify-content-center text-center ccc2">
              <img id="navimage" style="height: 70px;" 
                src="https://www.creativefabrica.com/wp-content/uploads/2021/03/20/Mountain-logo-Design-Graphics-9785421-1-580x435.png"
                alt="">
          </div>
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
  color: white;
}

div {
  color: white;
  background-color: black;
}

p {
  margin-top: 8px !important;
  margin-right: 46px !important;
}

.options {
  border-radius: 100px;
}

@media (min-width: 768px) {
  .options:hover {
    background-color: rgb(255, 255, 255);
    color: black !important;
  }
}

@media (max-width: 768px) {
  .options:hover {
    animation: changeColor 0.2s 1;
    color: white;
  }
}
@media screen and (max-width: 287px) {
  .ccc {
    justify-content: start !important;
  }
}

@media screen and (min-width: 576px) and (max-width: 630px) {
  .ccc2 {
    padding-left: 0 !important;
  }
}


@keyframes changeColor {

  0%,
  100% {
    color: #ffffff;
  }

  25%,
  75% {
    color: #b1b1b1;
  }

  50% {
    color: #8b8b8b;
  }
}


#navimage:hover {
  animation: sacudir 0.5s ease 1;
}




@keyframes sacudir {
  0% {
    transform: translateX(0);
  }

  25% {
    transform: translateX(-3px) rotate(-3deg);
  }

  50% {
    transform: translateX(3px) rotate(3deg);
  }

  75% {
    transform: translateX(-3px) rotate(-3deg);
  }

  100% {
    transform: translateX(0);
  }
}


.bi-twitter:hover {
  filter: invert(46%) sepia(57%) saturate(1958%) hue-rotate(161deg) brightness(94%) contrast(101%);
}

.bi-facebook:hover {
  filter: invert(69%) sepia(52%) saturate(729%) hue-rotate(183deg) brightness(95%) contrast(84%);
}

.bi-telegram:hover {
  filter: invert(73%) sepia(79%) saturate(1176%) hue-rotate(171deg) brightness(104%) contrast(101%);
}

.bi-whatsapp:hover {
  filter: invert(15%) sepia(37%) saturate(826%) hue-rotate(87deg) brightness(87%) contrast(102%);
}
</style>