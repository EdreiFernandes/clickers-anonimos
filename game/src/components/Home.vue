<template>
  <div class="container text-center">
    <ul class="list-group list-group-flush">
      <li class="list-group-item my-5">
        <h2>Sejá bem vindo aos Clickers Anónimos</h2>
        <small v-if="contador > 0">Não clique em ai</small>
      </li>

      <li class="list-group-item">
        <app-botao v-on:ContarClick="aumentarContador($event)"></app-botao>
      </li>
    </ul>
  </div>
</template>

<script>
import Botao from "@/components/Botao.vue";

export default {
  components: {
    "app-botao": Botao,
  },
  data() {
    return {
      contador: 0,
    };
  },
  methods: {
    aumentarContador(_add) {
      this.contador += _add;
    },
  },
};
</script>

<style scoped>
</style>