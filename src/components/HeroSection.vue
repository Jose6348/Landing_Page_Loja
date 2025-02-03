<template>
    <section class="hero">
      <div class="hero-content">
        <h2>Bem-vindo à Nossa Landing Page</h2>
        <p>Descubra nossos serviços inovadores e de alta qualidade!</p>
        <BaseButton>Conheça Mais</BaseButton>
      </div>
    </section>
  </template>
  
  <script>
  import BaseButton from './base/Button.vue'
  
  export default {
    name: 'HeroSection',
    components: {
      BaseButton
    }
  }
  </script>
  
  <style scoped>
  .hero {
    background: linear-gradient(135deg, #007BFF 0%, #0056b3 100%);
    color: white;
    padding: 100px 20px;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 50vh;
  }
  
  .hero-content {
    max-width: 800px;
    margin: 0 auto;
  }
  
  .hero-content h2 {
    font-size: 2.5em;
    margin-bottom: 20px;
  }
  
  .hero-content p {
    font-size: 1.2em;
    margin-bottom: 30px;
  }
  
  @media (max-width: 768px) {
    .hero {
      padding: 50px 10px;
    }
  
    .hero-content h2 {
      font-size: 2em;
    }
  
    .hero-content p {
      font-size: 1em;
    }
  }
  </style>