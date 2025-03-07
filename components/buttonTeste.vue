<!-- estrutura do componente (HTML) -->
<template>
    <button class="button" @click="count++">Você clicou no botão {{ count }} vezes.</button>
</template>


<!-- JavaScript code -->
<script setup>
    // importa ref para criar variaveis reativas
    import { ref } from 'vue'

    //variavel reativa que atualiza a tela automaticamente (não precisa de F5 e etc)
    const count = ref(0)
</script>

<!-- estilo do botão -->
<style> 
.button {
  background-color: #04AA6D; /* Green */
  border: none;
  border-radius: 20px;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>