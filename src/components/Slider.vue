<template>
  <Carousel :perPageCustom="[[768, 1], [1024, 3]]" :perPage="1">
    <Slide v-for="(slide, index) in slides" :key="index">
      <img :src="slide.src" alt="">
    </Slide>
  </Carousel>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel';

export default {
  name: 'Slider',
  data: () => {
    return {
        slides: [
            {src: require("../assets/1.jpeg")},
            {src: require("../assets/2.jpeg")},
            {src: require("../assets/3.jpeg")},
            {src: require("../assets/4.jpeg")},
            {src: require("../assets/5.jpeg")},
        ]
    }
  },
  components: {
    Carousel,
    Slide
  }
}
</script>

<style scoped>

</style>
