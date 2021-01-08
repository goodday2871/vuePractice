<template>
  <div id="app">
    <salutation v-model:salutation="form.salutation" v-model:name="form.name" />
    <pre>{{ form }}</pre>
  </div>
</template>

<script>
import salutation from "@/salutation";
import { reactive } from "vue";

export default {
  name: "App",
  components: {
    salutation,
  },
  data() {
    const form = reactive({
      salutation: "",
      name: "",
    });
  },
};
</script>

<style></style>
