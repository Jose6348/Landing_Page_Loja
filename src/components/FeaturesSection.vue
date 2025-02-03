<template>
    <section class="features">
      <div class="features-content">
        <h2>Características</h2>
        <div class="feature-list">
          <div v-for="feature in features" :key="feature.id" class="feature">
            <h3>{{ feature.title }}</h3>
            <p>{{ feature.description }}</p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'FeaturesSection',
    data() {
      return {
        features: [
          { id: 1, title: 'Feature 1', description: 'Descrição da Feature 1' },
          { id: 2, title: 'Feature 2', description: 'Descrição da Feature 2' },
          { id: 3, title: 'Feature 3', description: 'Descrição da Feature 3' }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  .features {
    padding: 50px 20px;
    background-color: #f4f4f4;
  }
  
  .features-content {
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .feature-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
  
  .feature {
    background: white;
    padding: 20px;
    margin: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    width: calc(33% - 40px);
    text-align: center;
  }
  
  .feature h3 {
    margin-top: 0;
  }
  
  @media (max-width: 768px) {
    .feature {
      width: 100%;
      margin: 10px 0;
    }
  }
  </style>