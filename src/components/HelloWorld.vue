<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <BaseAction href="https://google.fr">Link to Google</BaseAction>

    <BaseAction type="button">Just a button</BaseAction>
  </div>
</template>

<script setup lang="ts">
import { withDefaults, defineProps } from "vue";
import BaseAction from "./BaseAction.vue";

withDefaults(
  defineProps<{
    msg?: string;
  }>(),
  {
    msg: "Hello Default!",
  }
);
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
