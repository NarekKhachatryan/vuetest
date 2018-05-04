<template>
  <header>
    <NavBar/>
    <Slider/>
  </header>
</template>

<script>
import NavBar from './NavBar.vue'
import Slider from './Slider.vue'

export default {
  name: 'Header',
  components: {
    NavBar,
    Slider
  }
}
</script>

<style scoped>
  header {
    background-image: linear-gradient(#000000, #ffffff);
    min-height: 300px;
  }
</style>
