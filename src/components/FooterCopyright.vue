<script setup>



</script>


<template>
    <div class="container-fluid d-none d-sm-block">
        <div class="row">
            <div style="padding-top: 20px !important;" class="col-4">
                <span>© 2024 Company, Inc</span>
            </div>
            <div class="col-4">
                <img style="height: 70px !important;" class="img-fluid d-block mx-auto"
                    src="https://www.creativefabrica.com/wp-content/uploads/2021/03/20/Mountain-logo-Design-Graphics-9785421-1-580x435.png"
                    alt="">
            </div>
            <div style="padding-top: 20px !important;" class="col-4">
                <ul class="nav justify-content-around">
                    <li class="ms-3"><a title="hola" href=""><i class="bi bi-whatsapp" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-facebook" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-twitter" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-telegram" style="color: white;"></i></a></li>
                </ul>
            </div>
        </div>
    </div>

    <div class="container-fluid d-block d-sm-none">
        <div class="row">
            <div class="col-12 text-center">
                <img style="height: 70px !important;" class="img-fluid d-block mx-auto"
                    src="https://www.creativefabrica.com/wp-content/uploads/2021/03/20/Mountain-logo-Design-Graphics-9785421-1-580x435.png"
                    alt="">
            </div>
            <div style="padding-top: 30px !important;" class="col-12 text-center">
                <ul class="nav justify-content-around">
                    <li class="ms-3"><a href=""><i class="bi bi-whatsapp" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-facebook" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-twitter" style="color: white;"></i></a></li>
                    <li class="ms-3"><a href=""><i class="bi bi-telegram" style="color: white;"></i></a></li>
                </ul>
            </div>
            <div style="padding-top: 40px !important;" class="col-12 text-center">
                <span>© 2024 Company, Inc</span>
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


.container-fluid{
    padding: 50px 0 50px 0;
}


@media (max-width: 1199.98px) {
    .container-fluid {
        padding: 100px 0 20px 0;
    }
}

@media (max-width: 575.98px) {
    
.container-fluid{
    padding: 80px 0 20px 0;
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
</style>