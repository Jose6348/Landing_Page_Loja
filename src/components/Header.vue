<template>
    <header class="header">
      <div class="header-content">
        <h1>Minha Landing Page Profissional</h1>
        <nav>
          <ul>
            <li><a href="#" aria-label="Ir para Início">Início</a></li>
            <li><a href="#" aria-label="Sobre Nós">Sobre</a></li>
            <li><a href="#" aria-label="Contato">Contato</a></li>
          </ul>
        </nav>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header'
  }
  </script>
  
  <style scoped>
  .header {
    background-color: #333;
    color: white;
    padding: 1em 0;
    width: 100%;
    position: fixed;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
  }
  
  .header-content {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
  }
  
  .header nav ul {
    list-style: none;
    display: flex;
    padding: 0;
    margin: 0;
  }
  
  .header nav ul li {
    margin: 0 15px;
  }
  
  .header nav ul li a {
    color: white;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  .header nav ul li a:hover {
    color: #007BFF;
  }
  
  @media (max-width: 768px) {
    .header {
      padding: 0.5em 0;
    }
  
    .header-content {
      flex-direction: column;
      padding: 0 10px;
    }
  
    .header nav ul {
      flex-direction: column;
      align-items: center;
      margin-top: 10px;
    }
  
    .header nav ul li {
      margin: 5px 0;
    }
  }
  </style>