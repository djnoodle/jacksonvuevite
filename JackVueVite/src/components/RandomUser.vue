<script>
import jsonData from "/Users/nyber/OneDrive/Dokument/ITHS/VUE/VueClean/Vue/VueClean/jacksonvuevite/JackVueVite/public/jsonData.json";

export default {
  data() {
    return {
      data: jsonData,
    };
  },
};
</script>

<template>

    <div v-for="item in data" :key="item.id" id="jsonData">
        <label for="namn">Prudukt namn:</label>
        <p>{{ item.PruductName }}</p>
        <label for="pris">Pris:</label>
        <p>{{ item.Pris }}</p>
    </div>
</template>


