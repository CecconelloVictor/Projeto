<template>
    <div class="direito-trabalhista">
      <h2>Direito Trabalhista</h2>
      <label for="salario">Salário:</label>
      <input type="number" id="salario" v-model="salario" />
      <p>Imposto de Renda: {{ calcularImpostoDeRenda() }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        salario: 0
      };
    },
    methods: {
      calcularImpostoDeRenda() {
        if (this.salario <= 2000) {
          return "Isento";
        } else if (this.salario <= 5000) {
          return "10%";
        } else {
          return "20%";
        }
      }
    }
  };
  </script>
  
  <style scoped>
  .direito-trabalhista {
    max-width: 600px;
    margin: auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    font-family: Arial, sans-serif;
  }
  
  label {
    display: block;
    margin-bottom: 10px;
  }
  
  input[type="number"] {
    width: 100%;
    padding: 8px;
    box-sizing: border-box;
    margin-bottom: 20px;
  }
  
  p {
    font-weight: bold;
  }
  </style>