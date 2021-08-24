<template>
  <div id="header">
    <div class="container">
      <div class="row">
        <div class="col-sm-12 col-lg-3">
          <img src="../assets/photo.jpg" alt="">
        </div>
        <div class="col-sm-12 col-lg-9" >
          <h1>Romina Dehesa</h1>
          <h2>
            I am a <inline>Web Developer</inline> 
          </h2>
            <a v-on:click="show = !show">
              <inline v-if="show">ABOUT ME</inline><inline v-if="!show">CLOSE</inline>
            </a>
        </div>
        <div class="col-sm-12 col-lg-9" v-if="!show" id="about">
          <p>I'm 25 years old. I am from Argentina. I studied at the National University of the Center of the Province of Buenos Aires. In my studies, I acquired the necessary skills to build and develop quality applications or websites. In addition, I have acquired the experience of working under agile methodologies, such as Scrum.
          </p>
        </div>

        <div class="col-sm-12 col-lg-3" v-if="!show" id="about">
          <img src="../assets/profile.jpg" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      show: true,
    };
  },
};
</script>

<style>
#header {
  background-color: transparent;
  height: auto;
  text-align:end;
}
#header .container .row div{
  padding-bottom: 5%;
}
#header img {
  height: 250px;
  width: 250px;
  border-radius: 100%;
}
#header a {
  font-family: "Bebas Neue", cursive;
  border: none;
  color: black;
  padding: 10px;
  font-size: 20px;
  text-decoration: underline black;
}

#header h1, #header h2 {
  color: #3B5360;
  font-family: "Bebas Neue", cursive;
  font-size: 50px;
}

#header h1{
  font-family: 'Shadows Into Light', cursive;
  font-size: 100px;
  font-weight: bold;
  animation-name: t;
  animation-duration: 2s;
}
@keyframes t {
  0% {
    transform: scale(0);
  }
  100% {
    transform: scale(1);
  }
}
#header h2 inline {
  font-size: 70px;
}
#header div p {
  font-size: 30px;
  color: #3B5360;
}

#about {
  animation-duration: 3s;
  animation-name: a;
}

@keyframes a {
   from {
   opacity: 0.1
  }
  to {
    opacity: 1;
  }
}
</style>