<script>
export default {
  props: {
    imgSrc: String,
    series: {
      type: String,
      required: true,
    },
    price: {
      type: String, Number,
      required: true,
    },
    type: String,
  }
}
</script>

<template>
  <div class="single-card card h-100">
    <img :src="imgSrc" alt="" />

    <div class="text-white">
      {{ series }}
    </div>

    <div class="position-absolute attributes top">
      <span>{{ type }}</span>
    </div>
    <div class="position-absolute attributes bottom">
      <span>{{ price }}</span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.attributes {
  position: absolute;
  width: 100%;
  color: white;
  padding: 1rem 0;
  display: none;
  background-color: rgba(0, 0, 0, 0.650);
  text-align: center;
  width: 100%;
   
}
.top{
    top: 0;
   }
.bottom {
  bottom:0;
  background-color: rgba(0, 0, 0, 0.650);
}

.single-card:hover .attributes {
  display: block;
}

img {
  aspect-ratio: 1/1;
}
.card{
  background-color: transparent;
  border: 0;
}
</style>