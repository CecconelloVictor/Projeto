<template>
  <div class="component-wrapper">
    <h2>Lista de Clientes</h2>
    <div class="box">
      <p>Ver clientes cadastrados:</p>
      <button @click="verClientes">Ver Clientes</button>
    </div>
    <div class="box">
      <p>Cadastrar novo cliente:</p>
      <button @click="cadastrarCliente">Cadastrar Cliente</button>
    </div>
    <div class="box">
      <p>Ver andamento do processo:</p>
      <button @click="verAndamento">Ver Andamento</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    verClientes() {
      alert('Listar clientes cadastrados');
    },
    cadastrarCliente() {
      alert('Cadastrar novo cliente');
    },
    verAndamento() {
      alert('Ver andamento do processo de um cliente');
    }
  }
};
</script>

<style scoped>

</style>