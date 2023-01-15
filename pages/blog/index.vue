<template>
  <div>
    <main>
      <ul>
        <li v-for="blog in blogs" :key="blog.id">
          <nuxt-link :to="'/blog/' + blog.id">{{ blog.title }}</nuxt-link>
        </li>
      </ul>
    </main>
  </div>
</template>
  
  <script>
import axios from "axios";
export default {
  async asyncData() {
    const { data } = await axios.get("https://api.paulus-lestyo.my.id/blogs");
    console.log(data);
    return { blogs: data.blogs };
  },
};
</script>
  