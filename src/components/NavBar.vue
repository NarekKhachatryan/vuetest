<template>
  <nav>
    <ul>
      <li v-for="(item, index) in items" :key="index"><a :href="item.url">{{item.title}}</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
  data: () => {
    return {
        items: [
          {title: "Home", url: "#"},
          {title: "About Us", url: "#"},
          {title: "Contact Us", url: "#"}
        ]
    }
  }
}
</script>

<style scoped lang="stylus">
nav:after{
  display: block;
  content: "";
  clear: both;
  margin-bottom: 30px;
}
nav ul{
  list-style: none;
  margin: 0;
  padding: 0;
  width: 100%;
  background: #ccc;
  text-align: right;
}
li{
  display: inline-block;
}


nav a {
  color: #ffffff;
  padding: 0 20px;
  line-height: 40px;
}
</style>
