<template>
  <div class="playground">{{ info }}</div>
</template>

<script>
const axios = require("axios").default;

// axios.<method> will now provide autocomplete and parameter typings
export default {
  data() {
    return {
      info: null,
    };
  },
  beforeCreate() {
    axios
      .get("https://jsonplaceholder.typicode.com/todos/1")
      .then((response) => (this.info = response));
  },
};
</script>

<style></style>
