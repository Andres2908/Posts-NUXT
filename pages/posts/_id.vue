<template>
  <div class="card-color-dark">
    <h2 class="has-text-grey-lighter">{{ post.name }}</h2>
    <p>Id: {{ post.id }}</p>
    <p>Email: {{ post.email }}</p>
    <br />
    <p>{{ post.body }}</p>
  </div>
</template>

<script>
import axios from "axios";

export default {
  head() {
    return {
      title: "Editing Post ${this.$route.params.id}"
    };
  },
  data() {
    return {
      post: {}
    };
  },
  async created() {
    const res = await axios.get(
      "https://jsonplaceholder.typicode.com/comments/" + this.$route.params.id //De esta forma estamos recogiendo el id del URL
    );
    this.post = res.data;
  }
};
</script>

<style>
.card {
  border: 1px solid whitesmoke;
  padding: 4rem;
}
</style>
