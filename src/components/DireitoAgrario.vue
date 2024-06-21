<template>
  <div class="component-wrapper">
    <div class="direito-agrario">
      <h2>Direito Agrário</h2>
      <textarea v-model="descricaoAgraria" placeholder="Descrição do Caso Agrário"></textarea>
      <button @click="registrarCaso" class="primary-button">Registrar Caso</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      descricaoAgraria: ""
    };
  },
  methods: {
    registrarCaso() {
      console.log("Caso Agrário registrado:", this.descricaoAgraria);
      // Lógica para enviar dados do caso para o servidor
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

:root {
  --primary-color: #4CAF50;
  --primary-color-dark: #45a049;
  --background-color: #f9f9f9;
  --box-background-color: #fff;
  --box-border-color: #ccc;
  --text-color: #333;
  --header-color: #333;
  --highlight-color: #FF5733;
  --highlight-color-dark: #C13B23;
}

.component-wrapper {
  font-family: 'Roboto', sans-serif;
  background-color: var(--background-color);
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 800px;
  margin: 20px auto;
}

.direito-agrario {
  background-color: var(--box-background-color);
  padding: 20px;
  border: 1px solid var(--box-border-color);
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h2 {
  font-weight: 700;
  color: var(--header-color);
  margin-bottom: 20px;
}

textarea {
  width: 100%;
  height: 100px;
  padding: 10px;
  margin-bottom: 20px;
  box-sizing: border-box;
  border: 1px solid var(--box-border-color);
  border-radius: 5px;
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
}

button {
  padding: 10px 20px;
  background-color: var(--primary-color);
  color: rgb(50, 42, 91);
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: var(--primary-color-dark);
}

.primary-button {
  background-color: var(--highlight-color);
}

.primary-button:hover {
  background-color: var(--highlight-color-dark);
}
</style>
