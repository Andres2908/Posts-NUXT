<template>
  <div>
    <h1 class="has-text-grey-lighter">Posts</h1>
    <Post
      v-for="post of posts"
      v-bind:key="post.id"
      :id="post.id"
      :name="post.title"
      :content="post.content"
    />
  </div>
</template>

<script>
import axios from "axios";
import Post from "../../components/Post";

export default {
  components: {
    Post
  },
  data() {
    return {
      posts: []
    };
  },
  async created() {
    const res = await axios.get("https://jsonplaceholder.typicode.com/posts");

    this.posts = res.data;
    console.log(res);
  }
};
</script>

<style></style>
