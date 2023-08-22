<script>
export default {
    data() {
        return {
            navList: [
                { name: "characters".toUpperCase() },
                { name: "comics".toUpperCase() },
                { name: "movies".toUpperCase() },
                { name: "tv".toUpperCase() },
                { name: "games".toUpperCase() },
                { name: "collectibles".toUpperCase() },
                { name: "videos".toUpperCase() },
                { name: "fans".toUpperCase() },
                { name: "news".toUpperCase() },
                { name: "shop".toUpperCase() },
            ]
        }
    },

}

</script>


<template>
    <div class="d-flex justify-content-between align-item-center container">
        <div class="d-flex">
            <img src="../img/dc-logo.png" alt="">
        </div>
        <ul class="d-flex">
            <li class="itemList" v-for="listItem in navList"><a href="#">{{ listItem.name }}</a></li>
        </ul>
    </div>
</template>


<style scoped>
img {
    aspect-ratio: 1/1;
    height: 100px;
    margin: auto 0 auto 2rem;

}


li {
    list-style: none;
    padding: 3rem 1rem;
    font-size: 1.1rem;
    margin: auto 0;

    >a {
        color: black;
        text-decoration: none;
        font-weight: 600;
    }
}
</style>