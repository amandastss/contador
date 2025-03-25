<script setup>
import { ref } from 'vue';

const contador = ref(0);

function incrementar(){
  contador.value++
  
}
function decrementar(){
  contador.value--
}
function reiniciar(){
  contador.value = 0
}

</script>

<template>
<h1>
 Meu contador 2025
</h1>
<p>Valor do contador: {{ contador }}</p>
<button v-on:click="incrementar">+</button>
<button @click="decrementar">-</button>
<button @click="reiniciar">reiniciar</button>

</template>

<style scoped>

</style>
