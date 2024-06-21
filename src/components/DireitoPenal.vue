<template>
  <div class="processo-component">
    <h2>Andamento do Processo Penal</h2>
    <div class="andamento">
      <!-- Aqui você pode inserir o código para exibir o andamento do processo -->
      <ul>
        <li v-for="(evento, index) in eventos" :key="index">
          {{ evento.data }} - {{ evento.descricao }}
        </li>
      </ul>
    </div>

    <h2>Audiências</h2>
    <div class="audiencias">
      <!-- Aqui você pode inserir o código para exibir as audiências -->
      <ul>
        <li v-for="(audiencia, index) in audiencias" :key="index">
          {{ audiencia.data }} - {{ audiencia.horario }} - {{ audiencia.local }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      eventos: [
        { data: '01/01/2024', descricao: 'Petição inicial protocolada' },
        { data: '15/01/2024', descricao: 'Designação de audiência' },
        
      ],
      audiencias: [
        { data: '20/01/2024', horario: '09:00', local: 'Fórum Criminal' },
        { data: '05/02/2024', horario: '10:30', local: 'Tribunal de Júri' },
        
      ]
    };
  }
};
</script>

<style scoped>
.processo-component {
  font-family: Arial, sans-serif;
  border: 1px solid #ccc;
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 5px;
}

.andamento, .audiencias {
  margin-bottom: 15px;
}

ul {
  list-style-type: none;
  padding: 0;
}

ul li {
  margin-bottom: 5px;
  background-color: #d7bfbf;
  padding: 8px;
  border-radius: 3px;
}

ul li:nth-child(odd) {
  background-color: #ffffff;
}
</style>