<template>
  <div id="app">
    <carousel :autoplay="1500">
        <img class="carousel-cell" data-flickity-lazyload="https://placeimg.com/1000/600/any">
        <img class="carousel-cell" data-flickity-lazyload="https://placeimg.com/1000/600/any?2">
        <img class="carousel-cell" data-flickity-lazyload="https://placeimg.com/1000/600/any?5">
        <img class="carousel-cell" data-flickity-lazyload="https://placeimg.com/1000/600/any?4">
        <img class="carousel-cell" data-flickity-lazyload="https://placeimg.com/1000/600/any?3">
    </carousel>
    <router-link to="/" exact>home</router-link>
    <router-view />
  </div>
</template>

<script>
import Carousel from './components/Carousel.vue'

export default {
  name: 'App',
  components: {
    Carousel
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
