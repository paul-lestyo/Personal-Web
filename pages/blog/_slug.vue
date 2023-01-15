<template>
  <div>
    <main>
      <h1>{{ blog.title.toUpperCase() }}</h1>
		<p> {{ blog.text }} </p>
    </main>
  </div>
</template>
  
  <script>
import axios from "axios";
export default {
  async asyncData({params}) {
    const { data } = await axios.get(`https://api.paulus-lestyo.my.id/blogs/${params.slug}`);
    console.log(data);
    return { blog: data };
  },
};
</script>
  