<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <input type="checkbox" id="check" />
  <section class="home-section">
    <header class="home-header">
      <h2>
        <a href="#" class="home-logo">Mi granjita</a>
      </h2>
      <div class="home-navbar">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">Nosotros</RouterLink>
        <RouterLink to="/contact">Contacto</RouterLink>
      </div>
      <label class="home-label" for="check">
        <i class="fas fa-bars menu-btn"></i>
        <i class="fas fa-times close-btn"></i>
      </label>
    </header>
    <RouterView />
  </section>

</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}
</style>

<style scoped>
.home-section {
  position: relative;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
}
.home-header {
  position: absolute;
  top: 0;
  width: 100%;
  padding: 30px 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.home-logo {
  position: relative;
  color: #fc036b;
  font-size: 30px;
  text-decoration: none;
  text-transform: uppercase;
  font-weight: 800;
  letter-spacing: 1px;
}
.home-navbar * {
  text-decoration: none;
  font-weight: 500;
  letter-spacing: 1px;
  padding: 2px 15px;
  border-radius: 20px;
  transition: 0.3s;
  transition-property: background;
  color: #fc036b;
}
.home-navbar *:not(:last-child) {
  margin-right: 30px;
}
.home-navbar *:hover {
  background: #fc036b;
  color: #fff;
}
.home-label {
  display: none;
}
#check {
  z-index: 3;
  display: none;
}
/* Media Query */
@media only screen and (max-width: 960px) {
  .home-navbar {
    display: none;
  }
  .home-label {
    display: block;
    font-size: 25px;
    cursor: pointer;
    transition: 0.3s;
    transition-property: color;
  }
  .home-label:hover {
    color: #e75793;
  }
  .home-label .close-btn {
    display: none;
  }
  #check:checked ~ .home-section .home-header .home-navbar {
    z-index: 2;
    position: fixed;
    background: rgba(172, 68, 141, 0.9);
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  #check:checked ~ .home-section .home-header .home-navbar * {
    font-weight: 700;
    margin-right: 0;
    margin-bottom: 50px;
    letter-spacing: 2px;
  }
  #check:checked ~ .home-section .home-header .home-label .menu-btn {
    display: none;
  }
  #check:checked ~ .home-section .home-header .home-label .close-btn {
    z-index: 2;
    display: block;
    position: fixed;
  }
  .home-label .menu-btn {
    position: absolute;
  }
  .home-header .home-logo {
    position: absolute;
    bottom: -6px;
  }
}
</style>
