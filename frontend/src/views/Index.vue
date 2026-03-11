<script setup lang="ts">
import { ref } from 'vue'
import { useHead } from '@unhead/vue'
const tituloDinamico = ref('Home Page - Appointment Booker')
const descricaoDinamica = ref('Bem vindo a página home do sistema de ')

useHead({
  title: tituloDinamico,
  meta: [
    {
      name: 'description',
      content: descricaoDinamica
    },
    {
      property: 'og:title',
      content: tituloDinamico
    }
  ]
})
</script>

<template>
  <h1>Página Index.vue</h1>
</template>

<style scoped>

</style>
