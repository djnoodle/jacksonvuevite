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
    <h1>Coockie clicker v2</h1>
  <p><button @click="incrementValue">Increment Value</button></p>
  <p><button @click="decrementValue">Decrement Value</button></p>
  <p><button @click="resetValue">Reset Value</button></p>
  <h1>{{ counter }}</h1>
  <h1 v-if="counter > 10 && counter < 20">Bra start!</h1>
  <h1 v-if="counter > 100">Mus plattan är din!</h1>
  <h1 v-if="counter > 200">Tangentbordet!</h1>
  <h1 v-if="counter > 300">Ps4 är din!</h1>
  <h1 v-if="counter > 400">Ps5 är din!</h1>
  <h1 v-if="counter > 500">Frysen är din!</h1>
  <h1 v-if="counter > 600">Kylen är din!</h1>
  <h1 v-if="counter > 700">Tvm är din!</h1>
  <h1 v-if="counter > 800">skärmen är din!</h1>
  <h1 v-if="counter > 900">Laptopen är din!</h1>
  <h1 v-if="counter > 1000">Datorn är din!!!!!!!!</h1>
  <h1 v-if="counter < -10">Du går åt fel håll!</h1>
</template>
