<template>
  <div class="playground">{{ info }}</div>
</template>

<script>
// axios.<method> will now provide autocomplete and parameter typings
export default {
  data() {
    return {
      info: null,
    };
  },
  async mounted() {
    try {
      const response = await fetch(
        "https://jsonplaceholder.typicode.com/todos/1"
      );
      if (!response.ok) {
        const message = "Error with Status Code: " + response.status;
        throw new Error(message);
      }
      const data = await response.json();
      console.log(data);
    } catch (error) {
      console.log("Error: " + error);
    }
  },
};
</script>

<style></style>
