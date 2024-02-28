<script setup>



</script>


<template>
    <div class="container-fluidd">
    <div class="container-fluid">
        <div class="row">
            <div
                class="copy col-sm-4 col-lg-4 col-xl-12 col-xs-12 text-center text-sm-start text-xl-center order-xl-3 order-xs-1">
                <span>© 2024 Company, Inc</span>
            </div>
            <div class="imagen col-sm-4 col-lg-4 col-xl-12 col-xs-12 text-xl-center text-xs-center order-xl-1 order-xs-3">
                <img id="imgfooter" style="height: 70px !important;" class="img-fluid d-block mx-auto"
                    src="https://www.creativefabrica.com/wp-content/uploads/2021/03/20/Mountain-logo-Design-Graphics-9785421-1-580x435.png"
                    alt="">
            </div>
            <div class="contact col-sm-4 col-lg-4 col-xl-12 col-xs-12 text-xl-center text-xs-center order-xl-2 order-xs-2">
                <ul class="nav justify-content-around">
                    <li class="ms-3"><a href=""><i class="bi bi-whatsapp" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-facebook" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-twitter" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-telegram" style="color: white;"></i></a></li>
                </ul>
            </div>
        </div>
    </div>
</div>
</template>


<style scoped>
div {
    background-color: black;
    color: white;
    padding: 0 20px 0 20px;
}

.container-fluid {
    padding: 50px 0 50px 0;
}

.copy,
.contact{
    padding-top: 15px;
}

@media (max-width: 575.98px) {

    .contact,
    .copy {
        padding-top: 15px !important;
    }
    
    .imagen{
        padding-top: 23px !important;
    }
}

@media (min-width: 1199.98px) {
    .contact{
        padding: 30px 0 40px 0 !important;
    }
    .container-fluidd{
        padding: 0 !important;
    }
}


footer {
    border: 0 !important;
}

.row {
    margin: 0 !important;
    padding: 0 !important;
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




#imgfooter:hover {
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
</style>