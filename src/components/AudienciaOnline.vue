<template>
  <div class="component-wrapper">
    <h2>Juizado Especial</h2>
    <p>O juizado especial é uma unidade do Poder Judiciário que tem como objetivo proporcionar uma justiça mais rápida e simplificada para resolver causas de menor complexidade, geralmente de até 40 salários mínimos. Ele abrange diversas áreas do direito civil, como ações de cobrança, despejo para uso próprio, entre outras.</p>
    <p>Os procedimentos no juizado especial são menos formais e as partes podem representar-se a si mesmas (sem advogado) em muitos casos.</p>

    <div class="box">
      <p>Ver audiências:</p>
      <button @click="verAudiencias" class="highlight-button">Ver Audiências</button>
    </div>
    <div class="box">
      <p>Participar de audiências:</p>
      <button @click="participarAudiencias" class="highlight-button">Participar</button>
    </div>
    <div class="box">
      <p>Marcar horários de atendimento:</p>
      <button @click="marcarAtendimento" class="highlight-button">Marcar Atendimento</button>
    </div>
    
    <div class="black-box">
      <h3>Consultar Processos e Ver Audiências</h3>
      <div class="box">
        <p>Consultar processos:</p>
        <button @click="consultarProcessos">Consultar Processos</button>
      </div>
      <div class="box">
        <p>Ver audiências:</p>
        <button @click="verAudienciasBlackBox">Ver Audiências</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    verAudiencias() {
      alert('Listar audiências do Juizado Especial');
    },
    participarAudiencias() {
      alert('Participar de audiências no Juizado Especial');
    },
    marcarAtendimento() {
      alert('Marcar horário de atendimento no Juizado Especial');
    },
    consultarProcessos() {
      alert('Consultar processos do Juizado Especial');
    },
    verAudienciasBlackBox() {
      alert('Ver audiências do Juizado Especial na caixa preta');
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

:root {
  --primary-color: #007BFF;
  --primary-color-dark: #0056b3;
  --highlight-color: #FF5733;
  --highlight-color-dark: #C13B23;
  --background-color: #f9f9f9;
  --box-background-color: #fff;
  --box-border-color: #ccc;
  --text-color: #333;
  --header-color: #333;
  --black-box-background: #000;
  --black-box-text: #fff;
}

.component-wrapper {
  font-family: 'Roboto', sans-serif;
  margin: 20px;
  padding: 20px;
  background-color: var(--background-color);
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  color: var(--text-color);
}

h2 {
  font-weight: 700;
  margin-bottom: 20px;
  color: var(--header-color);
}

p {
  font-weight: 400;
  line-height: 1.6;
  margin-bottom: 10px;
}

.box {
  border: 1px solid var(--box-border-color);
  padding: 15px;
  margin-bottom: 15px;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  background-color: var(--box-background-color);
}

button {
  background-color: var(--primary-color);
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  border-radius: 4px;
  font-size: 16px;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: var(--primary-color-dark);
}

.highlight-button {
  background-color: var(--highlight-color);
}

.highlight-button:hover {
  background-color: var(--highlight-color-dark);
}

.black-box {
  background-color: var(--black-box-background);
  color: var(--black-box-text);
  padding: 20px;
  margin-top: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.black-box h3 {
  margin-bottom: 20px;
}

.black-box .box {
  background-color: var(--black-box-background);
  border-color: var(--box-border-color);
}

.black-box button {
  background-color: var(--highlight-color);
}

.black-box button:hover {
  background-color: var(--highlight-color-dark);
}
</style>
