<script>
import { ref, onMounted } from "vue";

export default {
  setup() {
    const name = ref("");
    const el = ref();
    const submitForm = () => {
      console.log(`Formuläret Inskickad! Namn = ${name.value}`);
    };

    onMounted(() => {
      el.value.focus();
    });

    return {
      name,
      submitForm,
      el,
    };
  },
};
</script>

<template>
  <div class="centered">
    <div id="input">
      <h1>Hej {{ name }}</h1>
      <input ref="el" type="text" placeholder="Namn" v-model="name" />
      <div>
        <button @click="submitForm" :disabled="name.length <= 1">Submit</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
#input {
  margin: 0 auto;
  height: auto;
  overflow-x: hidden;
  color: black;
}
</style>
