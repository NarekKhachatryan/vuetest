<template>
  <div>
    <Header/>
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import Header from './Header.vue'

export default {
  name: 'Main',
  props: {
    msg: String
  },
  components: {
    Header
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
a {
  color: #42b983;
}
</style>
