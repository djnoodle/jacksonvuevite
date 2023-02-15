<script>
import jsonData from "../assets/jsonData.json";

export default {
  data() {
    return {
      data: jsonData,
    };
  },
  props: {
    RandomuserText: {
      type: String,
      required: true,
      default: "[Loading]",
    },
  },
};
</script>

<template>
  <div v-for="item in data" :key="item.id" id="jsonData">
    <label for="namn">{{ RandomuserText }}</label>
    <p>{{ item.PruductName }}</p>
    <label for="pris">Pris:</label>
    <p>{{ item.Pris }}</p>
  </div>
</template>
