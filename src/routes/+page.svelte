<script>
  // Nada específico no script para esta página
</script>

<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
  }

  header {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
  }

  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 80vh;
    flex-direction: column;
  }

  .container h2 {
    margin-bottom: 20px;
    font-size: 2em;
    color: #333;
  }

  .btn {
    background-color: #007bff;
    color: white;
    padding: 15px 30px;
    margin: 10px;
    border-radius: 8px;
    font-size: 1.2em;
    cursor: pointer;
    text-decoration: none;
    width: 200px;
    text-align: center;
  }

  .btn:hover {
    background-color: #0056b3;
  }
</style>

<header>
  <h1>Catálogo de Motos</h1>
</header>

<div class="container">
  <h2>Bem-vindo ao nosso Catálogo de Motos!</h2>
  <!-- Links para as outras seções -->
  <a href="/catalogo" class="btn">Ver Catálogo</a>
  <a href="/detalhes" class="btn">Detalhes das Motos</a>
  <a href="/preco" class="btn">Preços das Motos</a>
</div>
