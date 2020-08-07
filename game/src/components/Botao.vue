<template>
  <div>
    <button
      type="button"
      name="naoClica"
      id="naoClica"
      class="btn rounded-circle"
      @click="clicando()"
    >
      <img src="@/assets/ca.jpg" class="rounded-circle" title="Não Clique!" />
    </button>
  </div>
</template>

<script>
export default {
  props: {
    acrescimo: {
      type: Number,
      default: 1,
    },
  },
  methods: {
    clicando() {
      this.$emit("ContarClick", this.acrescimo);
    },
  },
};
</script>

<style scoped>
</style>