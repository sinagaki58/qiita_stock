<template>
  <div class="container">
    <h1 v-if="error.statusCode === 404">Page not found ...(☍﹏⁰)</h1>
    <h1 v-else>An error occured</h1>
    <nuxt-link to="/">Back Top</nuxt-link>
  </div>
</template>

<script>
export default {
  props: ['error']
}
</script>

<style scoped>
.container {
  padding-top: 10%;
  text-align: center;
}

h1 {
  font-size: 22px;
}
</style>
