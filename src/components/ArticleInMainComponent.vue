<template>
  <div class="article-box">
    <h3>{{ header }}</h3>
    <p>{{ text }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  name: "ArticleInMainComponent",
  props: ["headers", "texts"],
  data() {
    return {
      header: this.headers,
      text: this.texts,
    };
  },
});
</script>

<style scoped>
.article-box {
  color: white;
  margin-left: 200px;
  margin-right: 40px;
  margin-bottom: 40px;
  padding: 40px;
  padding-left: 50px;
  background-color: #161616 !important;
  white-space: pre-wrap;
}
h3 {
  font-weight: bold;
  color: orange;
}
p {
  width: 80%;
}
@media only screen and (max-width: 600px) {
  p {
    width: 100%;
  }
}
</style>