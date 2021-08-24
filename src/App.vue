<template>
  <div id="app">
    <div class="container">
      
      <div class="row">
        <Header/>
      </div>
      <div class="row">
        <Works/>
      </div>
      <div class="row">
        <Footer/>
      </div>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Works from './components/Works.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Works,
    Footer
  }
}
</script>

<style>
  #app {
  padding-top: 5%;
  padding-bottom: 5%;
  animation-name: app;
  animation-duration: 3s;
  }

  @keyframes app{
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }
</style>
