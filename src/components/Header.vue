<template>
  <div id="header" class="col-12">
    <img src="../assets/photo.jpg" alt="">
    <h1>Romina Dehesa</h1>
    <h2>I am a <inline>Web Developer</inline></h2>
    <h3 v-if="!show">
      My skills are PHP, MySQL, JAVA, HTLM, CSS, JS, among others.
    </h3>
    <button v-on:click="show = !show">
      <inline v-if="show">ABOUT ME</inline>
      <inline v-if="!show">CLOSE</inline>
    </button>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      show: false,
    };
  },
};
</script>

<style>
#header {
  background-color: transparent;
  height: auto;
}
#header img {
  width: 30%;
  height: 90%;
  border-radius: 100%;
  margin: 10px;
  float: left;
}
button {
  background-color: transparent;
  font-family: "Bebas Neue", cursive;
  float: right;
  border: 1px solid #3B5360;
  color: #3B5360;
  margin: 10px;
}

#header h1, #header h2, #header h3 {
  color: #3B5360;
  font-family: "Bebas Neue", cursive;
  margin: 10px;
  text-align: end;
  /*animation-duration: 2s;
  animation-name: msj;*/
}

#header h1{
  font-family: 'Shadows Into Light', cursive;
  font-size: 100px;
  font-weight: bold;
}
#header h2 inline {
  font-size: 50px;
}
/*
@keyframes msj {
  from {
    margin-left: 100%;
    width: 300%;
  }
  to {
    margin-left: 0%;
    width: 100%;
  }
}*/
</style>