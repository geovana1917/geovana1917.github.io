<script>
    let motos = [
      {
        nome: "Honda CB 500X",
        preco: "R$ 29.990,00"
      },
      {
        nome: "Yamaha MT-03",
        preco: "R$ 23.990,00"
      }
    ];
  </script>
  
  <style>
    .precos {
      padding: 20px;
    }
  
    .preco-card {
      background-color: white;
      border-radius: 8px;
      padding: 15px;
      margin-bottom: 15px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
  
    .preco-card h3 {
      margin: 0;
      font-size: 1.3em;
    }
  
    .preco-card p {
      font-size: 1.2em;
      color: #333;
    }
  </style>
  
  <h2>Preços das Motos</h2>
  
  <div class="precos">
    {#each motos as moto}
      <div class="preco-card">
        <h3>{moto.nome}</h3>
        <p><strong>Preço:</strong> {moto.preco}</p>
      </div>
    {/each}
  </div>
  