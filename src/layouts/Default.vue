<template>
  <div class="container">
    <div class="navigation">
      <Nav />
    </div>
    <div class="layout">
      <slot/>
    </div>
  </div>
</template>

<script>
import Nav from './Nav';

export default {
  name: 'App',
  components: {
    Nav
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Balthazar&family=Nunito&display=swap');
body {
  font-family: 'Nunito', serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}
.layout {
  max-width: 1440px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}
h1, h2, h3 {
  font-family: 'Balthazar', serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
h1 {
  font-size: 32px;
}
</style>
