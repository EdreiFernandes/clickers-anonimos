<template>
  <div class="container text-center">
    <ul class="list-group list-group-flush">
      <li class="list-group-item my-5">
        <h2>Sejá bem vindo aos Clickers Anónimos</h2>
        <!-- <small>Não clique em nada</small> -->
      </li>

      <li class="list-group-item">
        <app-botao></app-botao>
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
};
</script>

<style scoped>
</style>