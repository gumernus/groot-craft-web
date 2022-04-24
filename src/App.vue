<template>
<div style="padding-bottom: 80px;"></div>
  <NavbarComponent></NavbarComponent>
</template>

<script lang="ts">
import "bootstrap/dist/css/bootstrap.min.css";
import { defineComponent } from 'vue';
import NavbarComponent from "@/components/Navbar.vue"

export default defineComponent({
  name: 'App',
  components: {
    NavbarComponent
  },
});
</script>

<style>
*{
color: white;
}
a {
  color: rgb(255, 255, 255) !important;
}
a:hover{
  color: orange !important;
}
body{
background: #101010 !important;
}

</style>
