<template>
    <footer class="footer" aria-label="Rodapé do site">
      <div class="footer-content">
        <p>© 2025 Minha Empresa. Todos os direitos reservados.</p>
        <nav>
          <ul>
            <li><a href="#" aria-label="Política de Privacidade">Privacidade</a></li>
            <li><a href="#" aria-label="Termos de Serviço">Termos</a></li>
            <li><a href="#" aria-label="Contato">Contato</a></li>
          </ul>
        </nav>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  .footer {
    background-color: #333;
    color: white;
    padding: 20px 0;
    text-align: center;
    width: 100%;
    position: relative;
    bottom: 0;
    animation: fadeIn ease 3s;
  }
  
  @keyframes fadeIn {
    0% { opacity: 0; }
    100% { opacity: 1; }
  }
  
  .footer-content {
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .footer nav {
    margin-top: 10px;
  }
  
  .footer nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    justify-content: center;
  }
  
  .footer nav ul li {
    margin: 0 10px;
  }
  
  .footer nav ul li a {
    color: white;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  .footer nav ul li a:hover {
    color: #007BFF;
  }
  
  @media (max-width: 768px) {
    .footer {
      padding: 10px 0;
    }
  
    .footer nav ul {
      flex-direction: column;
      align-items: center;
    }
  
    .footer nav ul li {
      margin: 5px 0;
    }
  }
  </style>