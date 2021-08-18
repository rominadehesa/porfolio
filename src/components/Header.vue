<template>
    <div id="img" class="col-12">
      <p> Hello World! </p>
      <p> My name is Romina Dehesa and I am a Web Developer.</p>
      <p v-if="!show">My skills are PHP, MySQL, JAVA, HTLM, CSS, JS, among others.</p>
      <button v-on:click="show = !show">
      <inline v-if="show">Ver mas</inline>
      <inline v-if="!show">Ver menos</inline>
      </button>
      
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
    height: auto;
    margin:10px;
    background-image: url('https://cdn.pixabay.com/photo/2015/04/20/13/17/work-731198_640.jpg');
    background-size: cover;
    text-align: center;
  }
  button{
    background-color: transparent;
    font-family: 'Bebas Neue', cursive;
    border: 1px solid white;
    color: white;
    margin:5px;
  }

  #img p{
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