<script setup>
import FooterCopyright from "../components/FooterCopyright.vue"
import FooterContact from "../components/FooterContact.vue" 
</script>



<template>
    <div style="padding-top: 100px;">
        <div class="container-fluid">
            <div class="row">
                <div class=" navf col-xl-6 col-md-12">
                    <FooterCopyright />
                </div>
                <div class="col-xl-6 col-md-12">
                    <div class="container">
                        <div class="">
                            <FooterContact />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>



<style scoped>
row {
    margin: 0 !important;
    padding: 0 !important;
}

.col-xl-6 {
    padding: 0 !important;
}

.col-md-12 {
    padding: 0 !important;
}

div{
    background-color: black !important;
}

.navf {
    padding-top: 50px !important;
}
</style>