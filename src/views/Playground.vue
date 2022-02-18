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
  async mounted() {
    try {
      this.info = await axios.get(
        "http://localhost:8080/api/profile-service/lookups"
      );
    } catch (err) {
      // Handle Error Here
      console.error(err);
    }
  },
};
</script>

<style></style>
