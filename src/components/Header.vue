<template>
    <div class="col-sm-4 col-md-4 col-lg-6" v-on:click="show = !show">
    <div id="img"></div>
    </div>
    <div class="colsm-8 col-md-8 col-lg-6">
    <p id="p" v-if="show">Desarrollo Web</p>
    </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
     return {
      show: true,
     }
  }
}
</script>

<style>
  #img {
    width: 150px;
    height: 150px;
    margin:10px;
    background-color: yellow;
    background-size: cover;
  }
  #p {
    color: #553C8B;
    font-family: 'Bebas Neue', cursive; 
    font-size: 20px;
    margin: 10px;
    text-align: center;
    font-weight: bold;
    animation-duration: 2s;
    animation-name: msj;
  }
  @keyframes msj {
    from {
      margin-left: 100%;
      width: 300%;
    }
    to {
      margin-left: 0%;
      width: 100%;
    }
  }
</style>