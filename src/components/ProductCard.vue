<script>
export default{
   props:{
    imgSrc:String,
    series:{
        type:String,
        required:true,  
    },
    price:{
        type:String,number,
        required:true,  
    },
    type:String,
   }
}
</script>

<template>

<div class="card h-100">
    <img :src="imgSrc" alt="" />

    <div class="card-body text-secondary">
      {{ series }}
    </div>

    <div class="overlay">
      <span>{{ type }}</span>
      <span>{{ price }}</span>
    </div>
  </div>

</template>

<style lang="scss" scoped>

</style>