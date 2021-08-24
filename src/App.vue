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
    background: rgb(232,234,230);
background: linear-gradient(90deg, rgba(232,234,230,1) 0%, rgba(205,208,203,0.6250875350140056) 87%);
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
