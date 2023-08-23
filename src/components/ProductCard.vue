<script>
export default{
    props: {
    imgSrc: String,
    series: {
      type: String,
      required: true,
    },
    price: [String, Number],
    type: String,
  },

}
</script>

<template>

<div class="card border-0 rounded-0 h-100 position-relative">
    <img :src="thumb" alt="" />

    <div class="card-body text-secondary">
      {{ series.toUpperCase() }}
    </div>

    <div class="overlay">
      <span> {{ type.toUpperCase() }}</span>
      <span> {{ price }}</span>
    </div>
  </div>
</template>

<style scoped>

</style>