<template>
    <div class="q-pa-md">
      <q-carousel
        animated
        v-model="slide"
        arrows
        navigation
        infinite
      >
        <q-carousel-slide :name="1" img-src="https://madeforhmns.com/cdn/shop/files/Alpha1.png?v=1683204675" class="carousel-img" />
        <q-carousel-slide :name="2" img-src="https://www.beautyhaul.com/assets/uploads/09._parfum_viral_tiktok_.jpg" class="carousel-img" />
        <q-carousel-slide :name="3" img-src="https://www.yslbeauty.co.id/dw/image/v2/BFZM_PRD/on/demandware.static/-/Sites-ysl-master-catalog/in_ID/dw7c56eb40/Fragrance/Y_EDP/WW-50194YSL_y-eau-de-parfum_ing-alt3_v2.jpg?sw=465&sh=465&sm=cut&sfrm=png&q=85" />
        <q-carousel-slide :name="4" img-src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRk3jOO4fD1XgeM6Oze4T6lleOIVlV8nqDtUuoEms2nOpZEGrU-wpMPIvgBQExuz-COako&usqp=CAU" class="carousel-img" />
      </q-carousel>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue'
  
  export default {
    setup () {
      return {
        slide: ref(1)
      }
    }
  }
  </script>
  
  <style scoped>
  .carousel-img {
    height: 400px; /* Ubah sesuai kebutuhan */
    background-size: cover;
    background-position: center;
  }
  </style>
  