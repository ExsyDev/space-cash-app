<template>
  <div>
    <Header />
    <main>
      <Nuxt />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style>
/* Global styles can be added here */
body {
  margin: 0;
  font-family: 'Arial', sans-serif;
  background-color: #0b0f19;
  color: #fff;
}
</style>
