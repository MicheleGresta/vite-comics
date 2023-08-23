<script>
import ProductCard from './components/ProductCard.vue';
import ProductsList from './db/dc-comics';

export default {
    components: {
        ProductCard,
    },
    data() {
    return {
      ProductsList
    };
  },
}
</script>

<template>
    <div class="cards-section">
        <div class="container">
            <div class="card-title">
                <h4> CURRENT SERIES</h4>
            </div>

            <div class="row row-cols-6 g-3">
                <div class="col" v-for="(product, i) in ProductsList" :key="`product_${i}`">
                    <ProductCard 
                    :img-src="ProductsList.thumb" 
                    :product-series="ProductsList.series" 
                    :product-price="ProductsList.price"
                    :product-type="ProductsList.type"
                    >
                    </ProductCard>
                </div>

            </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

.cards-section {
    background-color: rgb(48, 48, 48);
    min-height: 50px;

    .card-title {

        position: relative;

        h4 {
            background-color: $color-primary;
            padding: .6rem 1rem;
            color: white;
            font-weight: 600;
            position: absolute;
            top: -25px;
            left: 2rem;
        }

    }

    ;
}

;
</style>