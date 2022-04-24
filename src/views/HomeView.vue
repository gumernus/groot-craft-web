<template>
<div style="padding-bottom: 40px;"></div>

<div class="sidenav">
  <a href="#about">Eventy</a>
  <a href="#services">Soutěže</a>
  <a href="#clients">Updaty</a>
  <a href="#contact">Oznámení</a>
</div>

<div class="main">
<ArticleInMainComponent headers="Novinky na serveru" texts="⚜️ Vážení členové serveru, vážená komunito. ⚜️
Rádi bychom vás informovali o novinkách na serveru. 
První a hlavní znatelná věc které si všimnete, je web který byl předělán a dostal nový kabát. Naleznete zde všechny potřebné informace k..."></ArticleInMainComponent><ArticleInMainComponent headers="Novinky na serveru" texts="⚜️ Vážení členové serveru, vážená komunito. ⚜️
Rádi bychom vás informovali o novinkách na serveru. 
První a hlavní znatelná věc které si všimnete, je web který byl předělán a dostal nový kabát. Naleznete zde všechny potřebné informace k..."></ArticleInMainComponent><ArticleInMainComponent headers="Novinky na serveru" texts="⚜️ Vážení členové serveru, vážená komunito. ⚜️
Rádi bychom vás informovali o novinkách na serveru. 
První a hlavní znatelná věc které si všimnete, je web který byl předělán a dostal nový kabát. Naleznete zde všechny potřebné informace k..."></ArticleInMainComponent><ArticleInMainComponent headers="Novinky na serveru" texts="⚜️ Vážení členové serveru, vážená komunito. ⚜️
Rádi bychom vás informovali o novinkách na serveru. 
První a hlavní znatelná věc které si všimnete, je web který byl předělán a dostal nový kabát. Naleznete zde všechny potřebné informace k..."></ArticleInMainComponent>
</div>  

</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ArticleInMainComponent from '@/components/ArticleInMainComponent.vue';

export default defineComponent({
  name: 'HomeView',
  components: {
    ArticleInMainComponent
  },
});
</script>

<style scoped>
h1{
  color: white;
}


.sidenav {
  width: 260px;
  position: fixed;
  z-index: 1;
  top: 150px;
  left: 40px;
  background-color: #161616 !important;
  overflow-x: hidden;
  padding-top: 30px;
  padding-left: 30px;
  padding-bottom: 30px;
}

.sidenav a {
  padding: 5px 8px 6px 16px;
  text-decoration: none;
  font-size: 25px;
  color: white;
  display: block;
}

.sidenav a:hover {
  color: #064579;
}

.main {
  margin-left: 140px; /* Same width as the sidebar + left position in px */
  font-size: 28px; /* Increased text to enable scrolling */
  /* padding: 0px 10px; */
}

</style>