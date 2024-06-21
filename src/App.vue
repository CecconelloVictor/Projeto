
<template>
  <div> 
    <img alt="LOGO NOVA" src="./assets/LOGO NOVA.png">
    <HelloWorld />
    <ListaDeClientes />
    <DireitoPenal />
    <DireitoTrabalhista />
    <DireitoAgrario />
    <NovoProcesso />
    <!-- <JuizadoEspecial /> -->
    <AudienciaOnline />
    
  </div>
</template>

<script>

// import JuizadoEspecial from './components/JuizadoEspecial.vue';
import ListaDeClientes from './components/ListaDeClientes.vue';
import DireitoPenal from './components/DireitoPenal.vue';
import DireitoTrabalhista from './components/DireitoTrabalhista.vue';
import DireitoAgrario from './components/DireitoAgrario.vue';
import NovoProcesso from './components/NovoProcesso.vue';
import HelloWorld from './components/HelloWorld.vue';
import AudienciaOnline from './components/AudienciaOnline.vue';

export default {
  components: {
 
     ListaDeClientes, DireitoPenal, DireitoTrabalhista, DireitoAgrario, NovoProcesso, HelloWorld, AudienciaOnline}
  }
</script>

<style>

 #app {
  background-color: #bec2c0d3;
  font-family: Arial, sans-serif; 
   ;
  text-align: center;
  align-items: center;
  padding: 20px; 
}

  component-wrapper {
  width: 300px;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  font-family: Arial, sans-serif;
}
.audiencia-online {
  background-color: #000000; 
  border: 1px solid #8c171771;
}

.direito-agrario {
  background-color: #e8f5e9; 
  border: 1px solid #4caf50;
}

.direito-penal {
  background-color: #831238;
  border: 1px solid #e91e63;
}

.hello-world {
  background-color: #0c191b;
  border: 1px solid #00bcd4;
}

.lista-clientes {
  background-color: #8a1010; 
  border: 1px solid #ff5252;
}

.novo-processo {
  background-color: #c4c0c6; 
  border: 1px solid #1c141e40;
}

</style>


