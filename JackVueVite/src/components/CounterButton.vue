<script>
export default {
  data: function () {
    return {
      counter: 0,
    };
  },
  methods: {
    incrementValue() {
      this.counter++;
    },
    decrementValue() {
      this.counter--;
    },
    resetValue() {
      this.counter = 0;
    },
  },
};
</script>

<template>
  <p><button @click="incrementValue">Increment Value</button></p>
  <p><button @click="decrementValue">Decrement Value</button></p>
  <p><button @click="resetValue">Reset Value</button></p>
  <h1>{{ counter }}</h1>
  <h1 v-if="counter > 10">Nästan där!</h1>
  <h1 v-if="counter > 100">Winner!!!!!!!!!!!</h1>
  <h1 v-if="counter < -10">Du går åt fel håll!</h1>
</template>
