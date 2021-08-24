<template>
  <div id="header" class="col-12">
    <img src="../assets/photo.jpg" alt="">
    <h1> Hello World &lt;  y  &gt; </h1>
    <h2>My name is Romina Dehesa and I am a Web Developer.</h2>
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
  /*background-image: url('https://cdn.pixabay.com/photo/2015/07/02/10/45/woman-828953_960_720.jpg');*/
  background-color: transparent;
  background-size: cover;
  height: auto;
  margin-top: 10%;
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
  border: 1px solid #553C8B;
  color: #553C8B;
  margin: 10px;
}

#header h1, #header h2, #header h3 {
  color: #553C8B;
  font-family: "Bebas Neue", cursive;
  margin: 10px;
  text-align: end;
  font-weight: bold;
  font-size: 50px;
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