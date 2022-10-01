<template>
  <div class="container" :class="changeColor ? 'color1' : 'color2'">
    <h1>Iteration 5</h1>
    <h1>This Div changes it's COLOR</h1>
    <button @click="changeColorFunction">Click and See What Happens!</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const changeColor = ref(true);
function changeColorFunction() {
  changeColor.value = !changeColor.value;
}
</script>

<style>
.container {
  margin-top: 3rem;
  min-height: 5rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  text-align: center;
  color: black;
}
.color1 {
  background-color: rgb(167, 5, 72);
}
.color2 {
  background-color: rgb(68, 66, 184);
}
</style>
