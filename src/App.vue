<template>
  <label for="cor">Digite a cor no formato #FFFFFF</label>
  <input type="text" name="cor" id="cor" v-model="cor" placeholder="Digite a cor no formato #FFFFFF">
  <label for="tamanho_fonte">Digite o numero do tamanho da fonte</label>
  <input type="text" name="tamanho_fonte" id="tamanho_fonte" v-model="tamanho_fonte" placeholder="Digite o numero do tamanho da fonte">
  <label for="texto">Digite o texto</label>
  <input type="text" name="texto" id="texto" v-model="texto" placeholder="Digite o texto">
  <exe-3 >
    <p v-bind:style="{color: cor, fontSize: tamanho_fonte + 'px'} ">
        {{texto}}
    </p>
  </exe-3> 
  <!-- Valor default do componente -->
  <exe-3>
  </exe-3> 
<p></p>
<p></p>
<exe-4/>
</template>
<script>
import Exe3 from "./components/Exe3.vue";
import Exe4 from "./components/Exe4.vue";
export default {
  name: "App",
  components: {
    Exe3,
    Exe4
  },
  data: function(){
    return{
      cor: "#0000FF",
      tamanho_fonte: "44",
      texto: "Texto Slot"
    }
  }
};
</script>