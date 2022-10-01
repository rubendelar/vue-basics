<template>
  <div>
    <h1>Iteration 2</h1>
    <br />
    <h2>The sum of 2 + 2 equals to: {{ number1 + number2 }}</h2>
    <h2>Best way to do it: {{ 2 + 2 }}</h2>
    <h2>
      {{ printString }}
    </h2>
    <br />
    <br />
    <h1>Iteration 3</h1>
    <br />
    <h2 v-bind:class="iteration3 ? 'showUp' : 'notDisplay'">
      This element sets it's color to green and only shows up if the condition
      is set to true :)
    </h2>
    <h2 v-show="iteration3">
      (Best way to do it -v-show) This element only shows up if the condition is
      set to true :)
    </h2>

    <br />
    <br />
  </div>
</template>

<script setup>
import { ref } from "vue";
const number1 = ref(2);
const number2 = ref(2);
const iteration3 = ref(true);
const printString = () => {
  return "This appeared by executing a function!";
};
</script>

<style>
.showUp {
  color: green;
  font-weight: 500;
  /* font-size: 2rem; */
  top: -10px;
}
.notDisplay {
  display: none;
}
</style>
