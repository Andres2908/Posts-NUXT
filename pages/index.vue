<template>
  <div
    class="container has-background-link has-text-grey-lighter is-family-monospace"
  >
    <h1 class="title is-2 has-text-grey-lighter">
      Welcome to my first nuxt app
    </h1>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Application Nuxt Posts | Home",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Website about posts"
        }
      ],

      htmlAttrs: {
        lang: "es"
      }
    };
  }
};
</script>

<style></style>
