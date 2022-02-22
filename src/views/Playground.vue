<template>
  <div class="playground">{{ info }}</div>
</template>

<script>
// axios.<method> will now provide autocomplete and parameter typings
import axios from "axios";
import qs from "qs";
export default {
  data() {
    return {
      info: null,
    };
  },
  async mounted() {
    const url = "http://localhost:8080/connect/token";
    const data = {
      client_id: "iCoMed_Mobile_IOS",
      client_secret: "c@mEd3234_21!",
      grant_type: "client_credentials",
    };
    const options = {
      method: "POST",
      headers: { "content-type": "application/x-www-form-urlencoded" },
      data: qs.stringify(data),
      url,
    };
    let res = await axios(options);
    console.log(res.data);
  },
};
</script>

<style></style>
