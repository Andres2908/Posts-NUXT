<template>
  <div class="container has-background-link has-text-grey-lighter">
    <h1>About Us</h1>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptates
      veniam officia quam dignissimos, repellendus cum rem corrupti enim.
      Voluptatem nesciunt consectetur, cupiditate culpa mollitia dolorum
      excepturi accusamus nostrum magnam expedita.
    </p>
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
