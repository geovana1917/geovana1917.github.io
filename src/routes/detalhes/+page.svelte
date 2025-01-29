<script>
    let motos = [
      {
        nome: "Honda CB 500X",
        descricao: "Uma moto de aventura com design robusto e excelente desempenho.",
        detalhes: "Suspensão dianteira invertida, motor de 500cc, com 47 cv de potência."
      },
      {
        nome: "Yamaha MT-03",
        descricao: "Moto naked com motor potente e design agressivo.",
        detalhes: "Motor de 321cc, 42 cv de potência, ideal para quem busca performance."
      }
    ];
  </script>
  
  <style>
    .detalhes {
      padding: 20px;
    }
  
    .moto-detalhes {
      margin-bottom: 20px;
    }
  
    .moto-detalhes h3 {
      margin: 0;
      font-size: 1.5em;
    }
  
    .moto-detalhes p {
      margin: 5px 0;
      color: #666;
    }
  </style>
  
  <h2>Detalhes das Motos</h2>
  
  <div class="detalhes">
    {#each motos as moto}
      <div class="moto-detalhes">
        <h3>{moto.nome}</h3>
        <p><strong>Descrição:</strong> {moto.descricao}</p>
        <p><strong>Detalhes Técnicos:</strong> {moto.detalhes}</p>
      </div>
    {/each}
  </div>
  