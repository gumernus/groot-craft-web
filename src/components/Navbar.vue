<template>
<nav class="navbar fixed-top navbar-expand-lg navbar-dark bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">GrootCraft</a>

    <!-- <img class="navbar-brand" src="../assets/logo.png" alt="logo" height="50" width="120"> -->

    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#"><router-link to="/">Home</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link"><router-link to="/about">Novinky</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link"><router-link to="/store">Store</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link"><router-link to="/kontakty">Kontakty</router-link></a>
        </li>
        <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Pravidla
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
          <li class="nav-item">
          <a class="dropdown-item"><router-link to="/pravidla/minecraft">Minecraft</router-link></a>
        </li>
        <li class="nav-item">
          <a class="dropdown-item"><router-link to="/pravidla/discord">Discord</router-link></a>
        </li>
        <li class="nav-item">
          <a class="dropdown-item"><router-link to="/pravidla/teamspeak">Teamspeak</router-link></a>
        </li>
        <li class="nav-item">
          <a class="dropdown-item"><router-link to="/pravidla/GDPR">GDPR</router-link></a>
        </li>
        </div>
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Nábory
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
          <li class="nav-item">
          <a class="dropdown-item"><router-link to="/nábory/helper">Helper</router-link></a>
        </li>
        <li class="nav-item">
          <a class="dropdown-item"><router-link to="/nábory/builder">Builder</router-link></a>
        </li>
        <li class="nav-item">
          <a class="dropdown-item"><router-link to="/nábory/developer">Developer</router-link></a>
        </li>
        </div>
      </li>
      </ul>
    </div>
  </div>
</nav>
<router-view/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'NavbarComponent',
});
</script>

<style scoped>
.navbar {
    background-color: #161616 !important;
    padding: 10px;
    font-size: 17px;
}
.navbar-brand{
    font-weight: bold;
}
.navbar-light .navbar-nav .nav-link{
  color: #ffffff !important;
}
.dropdown-menu{
    background-color: #161616 !important;
}
.dropdown-item{
  color: #ffffff !important;
}
.dropdown-item.active, .dropdown-item:active{
  background-color: #161616 !important;
}
.dropdown-item:focus, .dropdown-item:hover{
  background-color: #161616 !important;
}
a{
    text-decoration: none;
}
a.router-link-exact-active {
    font-weight: bold;
  color: orange !important;
}
.navbar-light, .navbar-toggler{
  border: none;
  color: rgb(255, 255, 255);
}
.navbar-toggler-icon{
  color: white !important;
}
.navbar-toggler:focus{
  border: none !important;
  box-shadow: none !important;
}
@media only screen and (max-width: 991px) {
  .dropdown-menu {
    border: none !important;
  }
}
</style>