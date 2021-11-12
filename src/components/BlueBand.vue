<template>
    <div class="blueband_container container d-flex justify-content-around text_white">
        <div class="col-20 d-flex align-items-center">
            <img src="..\assets\buy-comics-digital-comics.png" alt="">
            <div class="d-flex px-2">DIGITAL COMICS</div>
        </div>

        <div class="col-20 d-flex align-items-center">
            <img src="..\assets\buy-comics-merchandise.png" alt="">
            <div class="d-flex px-2">DC MERCHANDISE</div>
        </div>

        <div class="col-20 d-flex align-items-center">
            <img src="..\assets\buy-comics-subscriptions.png" alt="">
            <div class="d-flex px-2">SUBSCRIPTION</div>
        </div>

        <div class="col-20 d-flex align-items-center">
            <img src="..\assets\buy-comics-shop-locator.png" alt="">
            <div class="d-flex px-2">COMIC SHOP LOCATOR</div>
        </div>

        <div class="col-20 d-flex align-items-center">
            <img src="..\assets\buy-dc-power-visa.svg" alt="">
            <div class="d-flex px-2">DC POWER VISA</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'BlueBand'
}
</script>

<style lang="scss">
    div.blueband_container>div {
        cursor: pointer;
    }
</style>