<template>
  <div>
    <div class="position-absolute d-flex h-100 w-100">
      <div class="col-6 text-center border border-success">
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

      <div class="col-6 bg-success text-light">ola</div>
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
      var cookie = this.guaranas;
      this.$cookies.set("pipoca", cookie);
    },
  },
  mounted() {
    var guaranas = this.$cookies.get("pipoca");
    if (guaranas != undefined) {
      this.guaranas = guaranas;
    }
  },
};
</script>

<style lang="scss" scoped></style>
