<script>
export default {
    data() {
        return {
            comicsList: [
                { name: "Characters" },
                { name: "Comics" },
                { name: "Movies" },
                { name: "Tv" },
                { name: "Games" },
                { name: "Videos" },
                { name: "News" },
            ],
            shopList: [
                { name: "Shop DC" },
                { name: "Shop DC Collectibles" },
            ],
            dcList: [
                { name: "Terms of Use" },
                { name: "Privacy policy (New)" },
                { name: "Ad Choices" },
                { name: "Advertising" },
                { name: "Jobs" },
                { name: "Subscriptions" },
                { name: "Talent Workshops" },
                { name: "CPSC Certificates" },
                { name: "Ratings" },
                { name: "Shop Help" },
                { name: "Contact Us" },
            ],
            sitesList: [
                { name: "DC" },
                { name: "MAD Magazine" },
                { name: "DC Kids" },
                { name: "DC Universe" },
                { name: "DC Power Visa" },
            ]
        }
    }
}
</script>

<template>
    <div class="footer-list">
        <div class="container d-flex">
            <div class="d-flex py-5">
                <div>
                    <ul>
                        <h4>DC COMICS</h4>
                        <li v-for="singleItem in comicsList"><a href="#">{{ singleItem.name }}</a></li>
                    </ul>
                    <ul>
                        <h4>SHOP</h4>
                        <li v-for="singleItem in shopList"><a href="#">{{ singleItem.name }}</a></li>
                    </ul>
                </div>
                <ul>
                    <h4>DC</h4>
                    <li v-for="singleItem in dcList"><a href="#">{{ singleItem.name }}</a></li>
                </ul>
                <ul>
                    <h4>SITES</h4>
                    <li v-for="singleItem in sitesList"><a href="#">{{ singleItem.name }}</a></li>
                </ul>
            </div>
            <div>
                <img src="../img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
    <div class="footer-contacts">
        <div class="container d-flex justify-content-between py-4">
            <div class="btn btn-style">SIGN-UP NOW!</div>
            <div class="contacts-container d-flex gap-3">
                <h4>FOLLOW US</h4>
                <a href="#"><img src="../img/footer-facebook.png" alt=""></a>
                <a href="#"><img src="../img/footer-twitter.png" alt=""></a>
                <a href="#"><img src="../img/footer-youtube.png" alt=""></a>
                <a href="#"><img src="../img/footer-pinterest.png" alt=""></a>
                <a href="#"><img src="../img/footer-periscope.png" alt=""></a>
            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">

@use "../styles/partials/variables" as *;
.footer-list {
    background-image: url(../img/footer-bg.jpg);

    >.container {
        position: relative;
        overflow: hidden;
    }
}

.footer-list h4 {
    font-weight: 700;
    color: white;
}

li {
    font-size: .8rem;
    padding: .1rem;
    list-style: none;
}

a {
    color: gray;
    text-decoration: none;
}

.footer-list img {
    position: absolute;
    top: -50px;
    right: 0;
    height: 500px;
    aspect-ratio: 1/1;
    object-fit: cover;
}
.footer-contacts{
    background-color: rgb(48, 48, 48);
}
.btn-style{
    color: white;
    font-weight: 600;
    border: 1px solid $color-primary;
    border-radius: 0;
    margin-left: 2rem;
}
.footer-contacts h4{
    color: $color-primary;
}
</style>