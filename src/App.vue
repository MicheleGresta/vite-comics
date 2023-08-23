<script>
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import TheMain from './components/TheMain.vue';
import ProductCardsSection from './components/ProductCardsSection.vue';

export default {
  components: {
    TheHeader,
    TheFooter,
    TheMain,
    ProductCardsSection,

  },
};
</script>

<template>
  <TheHeader />
  <ProductCardsSection />
  <TheMain />
  <TheFooter />
</template>

<style></style>
