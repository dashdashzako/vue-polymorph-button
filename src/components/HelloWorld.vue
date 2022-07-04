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
