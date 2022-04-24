<template>
<div style="padding-bottom: 50px;"></div>

<div class="card text-white bg-dark" style="width: 50rem;">
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>


</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ArticleComponent from "@/components/ArticleComponent.vue"

export default defineComponent({
  name: 'HomeView',
  components: {
    // ArticleComponent
  },
});
</script>

<style scoped>
h1{
  color: white;
}
.parent {
  border: 1px solid black;
  margin: 1rem;
  padding: 2rem 2rem;
  text-align: center;
}
.child {
  display: inline-block;
  border: 1px solid red;
  padding: 1rem 1rem;
  vertical-align: middle;
}

</style>