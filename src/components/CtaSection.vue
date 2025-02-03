<template>
    <section class="cta">
      <h2>Chamada para Ação</h2>
      <BaseButton @click="handleClick">Comece Agora</BaseButton>
    </section>
  </template>
  
  <script>
  import BaseButton from './base/Button.vue'
  
  export default {
    name: 'CtaSection',
    components: {
      BaseButton
    },
    methods: {
      handleClick() {
        alert('Você clicou no botão!');
      }
    }
  }
  </script>
  
  <style scoped>
  .cta {
    text-align: center;
    padding: 50px 20px;
    background-color: #eee;
  }
  
  .cta h2 {
    margin-bottom: 20px;
  }
  </style>