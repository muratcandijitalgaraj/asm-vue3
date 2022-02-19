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
  mounted() {
    fetch("https://mag.comed.com.tr/api/abp/api-definition", {
      mode: "no-cors",
      credentials: "include",
      method: "GET",
    })
      .then((response) => response.json())
      .then((json) => console.log(json))
      .catch((error) => console.log("Authorization failed : " + error.message));
  },
};
</script>

<style></style>
