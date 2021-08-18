<template>
  <div id="img" class="col-4">
    <img src="../assets/profile.jpg" alt="" />
  </div>
  <div id="img" class="col-8">
    <p>Hello World!</p>
    <p>My name is Romina Dehesa and I am a Web Developer.</p>
    <p v-if="!show">
      My skills are PHP, MySQL, JAVA, HTLM, CSS, JS, among others.
    </p>
    <button v-on:click="show = !show">
      <inline v-if="show">Ver mas</inline>
      <inline v-if="!show">Ver menos</inline>
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
#img {
  height: auto;
}

#img img {
  width: auto;
  height: 150px;
  margin: 10px;
  opacity: 0.8;
}
button {
  background-color: transparent;
  font-family: "Bebas Neue", cursive;
  border: 1px solid #553C8B;
  color: #553C8B;
  margin: 10px;
}

#img p {
  color: #553C8B;
  font-family: "Bebas Neue", cursive;
  font-size: 20px;
  margin: 10px;
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