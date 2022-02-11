<template>
  <Layout>
    <section class="center">
      <h1>Bookopoly</h1>
      <p>
        Gameboard with bookish prompts. Read em' all.
      </p>
    </section>
    <section>
      <Gameboard />
    </section>

    <!--/* Learn how to use images here: https://gridsome.org/docs/images 
    <g-image alt="Example image" src="~/favicon.png" width="135" />*/-->
    <!--/* <p class="home-links">
      <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
      <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
    </p> */-->

  </Layout>
</template>

<script>
import Gameboard from '~/components/Gameboard.vue'

export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    Gameboard
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
.center {
  text-align: center;
}
</style>
