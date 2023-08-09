<script setup lang="ts">
const carouselImages = [
  'https://picsum.photos/1300/500',
  'https://picsum.photos/1500/600',
  'https://picsum.photos/1300/450',
  'https://picsum.photos/1350/480'
]
</script>

<template>
  <v-carousel cycle height="400" show-arrows="hover" id="carousel">
    <v-carousel-item
      v-for="(image, i) in carouselImages"
      :src="image"
      :key="'carousel' + i"
      cover
    ></v-carousel-item>
  </v-carousel>
</template>
