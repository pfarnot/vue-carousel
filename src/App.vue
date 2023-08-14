<script>


import Carousel from './components/carousel/Carousel.vue'

export default {

  name: "App",
  components: { Carousel },
  data: () => ({
    slides: [
      "https://picsum.photos/id/1032/900/400",
      "https://picsum.photos/id/1033/900/400",
      "https://picsum.photos/id/1035/900/400",
      "https://picsum.photos/id/1036/900/400",
      "https://picsum.photos/id/1037/900/400",
    ]
  })
}

</script>

<template>
  <div class="carousel-container">
    <carousel :slides="slides" :interval="3000" controls indicators></carousel>
  </div>
</template>

<style scoped>
.carousel-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>
