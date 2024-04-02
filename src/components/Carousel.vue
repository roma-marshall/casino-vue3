<template>
  <Carousel :items-to-show="2" :autoplay="3000" :wrap-around="true">
    <Slide v-for="slide in 10" :key="slide">
      <div class="carousel__item">
        <img src="https://placehold.co/1280x720" class="border" alt="">
      </div>
    </Slide>
  </Carousel>
</template>

<script setup>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide } from 'vue3-carousel'
</script>