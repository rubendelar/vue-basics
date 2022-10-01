<script setup>
import Footer from "./components/Footer.vue";
import navvbar from "./components/navvbar.vue";
import Operations from "./components/Operations.vue";
import Post from "./components/Post.vue";
import ColorButton from "./components/ColorButton.vue";
</script>

<template>
  <div>
    <header>
      <navvbar />
    </header>

    <Operations />
    <Post />
    <ColorButton />

    <Footer />
  </div>
</template>

<style scoped></style>
