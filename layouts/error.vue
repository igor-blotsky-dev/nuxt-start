<template>
  <div
    class="container d-flex w-100 h-100 justify-content-center align-content-center"
  >
    <div class="">
      <h1 v-if="error.statusCode === 404">Page not found</h1>
      <h1 v-else>An error occurred</h1>
      <h1>
        <nuxt-link to="/">Home page</nuxt-link>
      </h1>
    </div>
  </div>
</template>

<script>
export default {
  props: ["error"],
  layout: "blog" // you can set a custom layout for the error page
};
</script>
