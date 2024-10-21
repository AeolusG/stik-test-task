<template>
  <section>
    <div class="container">
      <TheHeader />
      <TheCard />
    </div>
    <TheArticles class="container" />
  </section>
</template>

<script>
import TheArticles from "~/components/TheArticles.vue";

export default {
  name: "IndexPage",
};
</script>

<style>
body {
  margin: 0;
}
.container {
  margin-right: auto;
  margin-left: auto;
  max-width: fit-content;
}
</style>
