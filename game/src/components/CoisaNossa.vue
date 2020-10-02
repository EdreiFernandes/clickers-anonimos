<template>
  <div>
    <div class="position-absolute h-100 w-50 text-center border border-success">
      <div id="status" class="my-5">
        <h1>{{ guaranas }} Guaranás vendidos</h1>
      </div>

      <button type="button" class="btn mt-5">
        <img
          src="@/assets/guarana.png"
          class="img-fluid"
          @click="venderGuarana()"
        />
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      guaranas: 0,
    };
  },
  methods: {
    venderGuarana() {
      this.guaranas++;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>