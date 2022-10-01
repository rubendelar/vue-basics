<template>
  <div>
    <h1>Iteration 4</h1>
    <br />
    <ul v-for="post in listofElements" v-bind:key="post">
      <li>
        <h2>
          Post Title: <b> {{ post.title }} </b>
        </h2>
        <h3>Post Description: {{ post.description }}</h3>
        <p>Post Content: {{ post.content }}</p>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from "vue";
const listofElements = ref([
  {
    title: "Central banks rising Interest rates at maximum speed",
    description:
      "Now they say inflation is not temporary and they are hurrying to rise the interest rates at a vertiginous speed",
    content:
      "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Perferendis possimus eaque, assumenda nesciunt sit consectetur sequi minima unde sint, facere soluta cumque! Vitae maiores iusto fuga. Tempora, iure suscipit. Ad.",
  },
  {
    title: "Traveling during covid restrictions",
    description: "Here is the list of all my travells during 2020",
    content:
      "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quidem provident qui cumque velit totam inventore veritatis consectetur distinctio voluptas, eligendi fugiat molestiae exercitationem magnam error natus nihil esse sit excepturi?.",
  },
  {
    title: "Climate change crisis",
    description:
      "Here is what governments are implementing to combat climate change",
    content:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo alias enim ad esse accusamus quas commodi quam, porro dolor in voluptatum tempore, inventore quisquam reiciendis autem odit nihil distinctio id!",
  },
]);
</script>

<style scoped>
li {
  margin: 5px;
  padding-left: 10px;
}

h5,
p {
  margin: 5px;
  padding-left: 10px;
}
</style>
