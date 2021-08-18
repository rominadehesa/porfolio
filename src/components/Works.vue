<template>
    <div class="col-12 nav">
      <li v-on:click="show = !show">Works</li>
    </div>
    <div class="col-12 body" v-if="show">
      <div class="container">
        <div class="row">
          <div class="col-sm-12 col-lg-6">

            <div class="card">
              <div class="card-header">
               <img src="https://image.flaticon.com/icons/png/512/3036/3036398.png" alt="">
               <img src="https://image.flaticon.com/icons/png/512/288/288882.png" alt="">
              </div>
              <div class="card-body">
                <h5 class="card-title">Instituto IDC</h5>
                <p class="card-text">Instituto con cursos de diferentes areas educativas. Este sitio web cuenta con registro/inicio de sesion de usuarios, tanto administradores de la pagina como futuros alumnos. </p>
                <a href="https://github.com/rominadehesa/idc-php-vue" class="btn" title="codigo">
                  <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-code-slash" viewBox="0 0 16 16">
                  <path d="M10.478 1.647a.5.5 0 1 0-.956-.294l-4 13a.5.5 0 0 0 .956.294l4-13zM4.854 4.146a.5.5 0 0 1 0 .708L1.707 8l3.147 3.146a.5.5 0 0 1-.708.708l-3.5-3.5a.5.5 0 0 1 0-.708l3.5-3.5a.5.5 0 0 1 .708 0zm6.292 0a.5.5 0 0 0 0 .708L14.293 8l-3.147 3.146a.5.5 0 0 0 .708.708l3.5-3.5a.5.5 0 0 0 0-.708l-3.5-3.5a.5.5 0 0 0-.708 0z"/>
                  </svg>
                </a>
              </div>
            </div>
  
          </div>

          <div class="col-sm-12 col-lg-6">

            <div class="card">
              <div class="card-header">
              <img src="https://cdn.worldvectorlogo.com/logos/angular-icon.svg" alt="">
              </div>
              <div class="card-body">
                <h5 class="card-title">Huertanica</h5>
                <p class="card-text">Sitio web con carrito de compras para los productos que ofrece "Huertanica".</p>
                <a href="https://github.com/rominadehesa/huertanica-angular" class="btn" title="codigo">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-code-slash" viewBox="0 0 16 16">
                  <path d="M10.478 1.647a.5.5 0 1 0-.956-.294l-4 13a.5.5 0 0 0 .956.294l4-13zM4.854 4.146a.5.5 0 0 1 0 .708L1.707 8l3.147 3.146a.5.5 0 0 1-.708.708l-3.5-3.5a.5.5 0 0 1 0-.708l3.5-3.5a.5.5 0 0 1 .708 0zm6.292 0a.5.5 0 0 0 0 .708L14.293 8l-3.147 3.146a.5.5 0 0 0 .708.708l3.5-3.5a.5.5 0 0 0 0-.708l-3.5-3.5a.5.5 0 0 0-.708 0z"/>
                  </svg>
                </a> 
                <a href="https://huertanica-app.stackblitz.io/home" class="btn" title="vista">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-window" viewBox="0 0 16 16">
                <path d="M2.5 4a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1zm2-.5a.5.5 0 1 1-1 0 .5.5 0 0 1 1 0zm1 .5a.5.5 0 1 0 0-1 .5.5 0 0 0 0 1z"/>
                <path d="M2 1a2 2 0 0 0-2 2v10a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V3a2 2 0 0 0-2-2H2zm13 2v2H1V3a1 1 0 0 1 1-1h12a1 1 0 0 1 1 1zM2 14a1 1 0 0 1-1-1V6h14v7a1 1 0 0 1-1 1H2z"/>
              </svg>
                </a>
              </div>
            </div>
  
          </div>
          <div class="col-6">
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Works',
  data() {
     return {
      show: false,
     }
  }
}
</script>

<style>   
  .nav {
      background-color: #a2aadd;
      display: flex;
      justify-content: center;
      font-family: 'Bebas Neue', cursive; 
      font-size: 30px;
      text-decoration: none;
    }
  .nav li {
      list-style: none;
      text-align: center;
      color: #553C8B;
    }
  h1{
    font-family: 'Major Mono Display', monospace;
    font-size: 40px;
  }
  a{
    background-color: #553C8B;
    color: white;
    margin: 2px;
  }
  .card {
    margin: 5px 5px;
    border: none;
    text-align: center;
  }
  .card-header {
    background-color: white;
  }
  .card-header img{
    height: 50px;
    width: auto;
  }
  .card-body a svg{
    height: 20px;
    width: 20px;
  }
  .card a {
    border: 1px solid #eaeeed;
  }
  .card a:hover {
    background-color: #eaeeed; 
  }
</style>