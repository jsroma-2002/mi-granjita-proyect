<script setup></script>

<template>
  <header>
    <div class="header-content">
      <h2>Explora un entorno verdaderamente natural</h2>
      <div class="line"></div>
      <h1>Disfruta del campo</h1>
      <a href="" class="ctn">Learn More</a>
    </div>
  </header>

  <!--Features-->
  <section class="features">
    <div class="title">
      <h1>¿Que Ofrecemos?</h1>
      <div class="line"></div>
    </div>
    <div class="row">
      <div class="col">
        <img
          src="../assets/features-organic-products.jpg"
          alt="organic-products"
        />
        <h4>Productos Organicos</h4>
        <p>
          Ofrecemos una canasta de productos organicos a nuestros afiliados. 
          Todos estos productos procedientes nuestras granjas afilidadas garantizando altos estandares calidad y salubridad.
        </p>
        <a href="" class="ctn">Learn More</a>
      </div>
      <div class="col">
        <img
          src="../assets/features-family-travel.jpg"
          alt="organic-products"
        />
        <h4>Viajes en Familia</h4>
        <p>
          Nuestras granjas afiliadas proveen espacios ideales para paseos en famila. 
          Disfrute de paseos en famila en los paisajes que ofrecen nuestros paseos guiados 
        </p>
        <a href="" class="ctn">Learn More</a>
      </div>
    </div>
  </section>

  <section class="footer">
    <p>Made by Copyright © Upcinos</p>
    <p>Thanks for visit us. Take a cookie &#127850</p>
  </section>
</template>

<style scoped>
header {
  height: 100vh;
  background-image: url("../assets/home-page-imge.jpg");
  background-position: bottom;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
}

a {
  text-decoration: none;
}

.header-content {
  margin-bottom: 150px;
  color: whitesmoke;
  text-align: center;
}

.header-content h2 {
  font-size: 4vmin;
}

.line {
  width: 150px;
  height: 4px;
  background: #fc036b;
  margin: 10px auto;
  border-radius: 5px;
}

.header-content h1 {
  font-size: 7vmin;
  margin-top: 50px;
  margin-bottom: 30px;
}

.ctn {
  padding: 8px 15px;
  background: #fc036b;
  border-radius: 30px;
  color: whitesmoke;
}

section {
  width: 80%;
  margin: 80px auto;
}

.title {
  text-align: center;
  font-size: 4vmin;
  color: rgb(73, 73, 126);
}

.row{
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-between;
}

.row .col {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.row .col img {
  width: 750px;
  height: 450px;
  max-width: 90%;
}

.features .row{
  margin-top: 50px;
}

h4{
  font-size: 3vm;
  color: #484872;
  margin: 20px auto;
}

p{
   color: #7c7c7c;
   padding: 0px 40px;
}

.features .ctn{
  margin-top: 30px;
}

  .footer{
  width: 100%;
  min-height: 100px;
  padding: 20px 80px;
  margin: 0;
  background: #484872;
  text-align: center;
}

.footer p {
  color: whitesmoke;
  margin: 20px auto;
}

@media only screen and (max-width: 960px) {
  
  .row{
    flex-direction: column;
  }

  .row .col{
    margin: 20px auto;
  }

}

</style>
