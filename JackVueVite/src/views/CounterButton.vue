<script setup>
import CounterButton from "../components/CounterButton.vue";
import RandomUser from "../components/RandomUser.vue";
</script>

<script>
export default {
  data: () => ({
    text: "Pruduct namn:",
  }),
};
</script>

<template>
  <div class="centered">
    <CounterButton />
    <RandomUser :RandomuserText="text" />
  </div>
</template>

<style scoped></style>
