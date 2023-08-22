<script>
export default {

}
</script>

<template>
    <main>
        <div class="container">
            <div class="cards-group d-flex">
                <div class="single-card d-flex">
                    <div>
                        <img src="../img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <h5>DIGITAL COMICS</h5>
                </div>
                <div class="single-card d-flex">
                    <div>
                        <img src="../img/buy-comics-merchandise.png" alt="">
                    </div>
                    <h5>DC MERCHANDISE</h5>
                </div>
                <div class="single-card d-flex">
                    <div>
                        <img src="../img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <h5>SUBSCRIPTION</h5>
                </div>
                <div class="single-card d-flex">
                    <div>
                        <img src="../img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <h5>COMIC SHOP LOCATOR</h5>
                </div>
                <div class="single-card d-flex">
                    <div>
                        <img src="../img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <h5>DC POWER VISA</h5>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;
main {
    background-color: $color-primary;
}

.single-card{
    justify-content: center;
    align-items: center;
    gap: 1rem;
    padding: 1rem;
    margin: 1rem;
    color: white;
    cursor: pointer;
    
    img{
        height: 3rem;
    }
    h5{
        font-size: .8rem;
    }
}
.cards-group{
    margin-left: 2rem;
}

</style>