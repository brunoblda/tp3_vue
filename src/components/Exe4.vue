<template>
  <div>
    <label for="cor">Digite a cor do quadrado no formato #FFFFFF</label>
    <input
      type="text"
      name="cor"
      id="cor"
      v-model="cor_back"
    />
    <div class="square" v-bind:style="{ background: cor_back }"></div>
  </div>
</template>

<script>
export default {
  name: "Exe4",
  data: function () {
    return {
      cor_back: "#993399",
    };
  },
};
</script>

<style scoped>
.square {
  width: 70px;
  height: 70px;
  border: 1px solid #000;
}
</style>