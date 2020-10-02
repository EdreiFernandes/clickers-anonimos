<template>
  <div id="app">
    <app-coisa-nossa></app-coisa-nossa>
  </div>
</template>

<script>
import CoisaNossa from "@/components/CoisaNossa.vue";

export default {
  name: "App",
  components: {
    "app-coisa-nossa": CoisaNossa,
  },
};
</script>

<style>
</style>
