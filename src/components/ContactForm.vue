<template>
    <form @submit.prevent="submitForm" class="contact-form">
      <h2>Contato</h2>
      <label for="name">Nome:</label>
      <input type="text" id="name" v-model="name" required>
      
      <label for="email">Email:</label>
      <input type="email" id="email" v-model="email" required>
      
      <BaseButton type="submit">Enviar</BaseButton>
    </form>
  </template>
  
  <script>
  import BaseButton from './base/Button.vue'
  
  export default {
    name: 'ContactForm',
    components: {
      BaseButton
    },
    data() {
      return {
        name: '',
        email: ''
      }
    },
    methods: {
      submitForm() {
        console.log('Formulário enviado:', this.name, this.email);
        // Lógica para enviar o formulário
        this.name = '';
        this.email = '';
      }
    }
  }
  </script>
  
  <style scoped>
  .contact-form {
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    max-width: 500px;
    margin: 0 auto;
  }
  
  .contact-form label, .contact-form input, .contact-form button {
    display: block;
    width: 100%;
    margin: 10px 0;
  }
  
  .contact-form input {
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
  }
  </style>