<template>
  <p>
    <img
      v-bind:style="{
        'background-image':
          'url(' + require('../../assets/img/uploads/' + data.items[0].img),
      }"
    />
  </p>
</template>
<script>
import json from "./data.json";
export default {
  data() {
    return {
      data: json,
    };
    //return console.log(json);
  },
  /*computed: {
    images() {
      const images = this.data.items[0].img;
      console.log(images);
      return require("../../assets/img/uploads/${images}.jpg");
    },
  },*/
};
</script>