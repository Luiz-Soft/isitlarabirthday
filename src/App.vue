<template>
  <div id="app">
    <a class="title" v-if="isLaraBirthday">SIM</a>
    <a class="title" v-else>NÃO</a>
  </div>
</template>

<script>
import moment from "moment";
export default {
  name: "App",
  components: {},
  computed: {
    isLaraBirthday() {
      return moment().format("DD/MM") === "02/07";
    },
  },
};
</script>

<style>
.title {
  display: inline-block;
  margin-top: 200px;
  font-weight: bold;
  font-size: 120pt;
  font-family: Arial, sans-serif;
  text-decoration: none;
  cursor: default;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
</style>
