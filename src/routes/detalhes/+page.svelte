<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Catálogo de Motos</title>
  <style>
    .catalogo {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 20px;
      padding: 20px;
    }

    .moto-card {
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      padding: 15px;
    }

    .moto-card h3 {
      margin: 0;
      font-size: 1.5em;
    }

    .moto-card p {
      color: #666;
    }

    .moto-card .preco {
      font-weight: bold;
      font-size: 1.2em;
      margin-top: 10px;
      color: #333;
    }

    .moto-card .detalhes {
      font-size: 0.9em;
      color: #444;
      margin-top: 5px;
      font-style: italic;
    }
  </style>
</head>
<body>
  <h2>Catálogo de Motos</h2>

  <div class="catalogo" id="motoCatalogo"></div>

  <script>
    let motos = [
      {
        nome: "Honda CB 500X",
        descricao: "Uma moto de aventura com design robusto.",
        detalhes: "Motor de 471cc, excelente para viagens longas.",
      },
      {
        nome: "Yamaha MT-03",
        descricao: "Moto naked com motor potente.",
        detalhes: "Motor de 321cc, leve e ágil para o trânsito urbano.",
      },
      {
        nome: "Kawasaki Ninja 400",
        descricao: "Motocicleta esportiva com alto desempenho.",
        detalhes: "Motor de 399cc, ótima para altas velocidades e curvas.",
      },
      {
        nome: "Suzuki V-Strom 650",
        descricao: "Moto de aventura com excelente estabilidade.",
        detalhes: "Motor de 645cc, versátil para diferentes tipos de terreno.",
      },
      {
        nome: "BMW G 310 R",
        descricao: "Naked compacta, ágil e com ótimo custo-benefício.",
        detalhes: "Motor de 313cc, ideal para quem busca praticidade e estilo.",
      },
      {
        nome: "Ducati Scrambler 800",
        descricao: "Design clássico e motor de alto desempenho.",
        detalhes: "Motor de 803cc, excelente para aventuras e pilotagem urbana.",
      },
      {
        nome: "Harley-Davidson Iron 883",
        descricao: "Cruiser com motor potente e visual icônico.",
        detalhes: "Motor de 883cc, famosa pela experiência de pilotagem única.",
      },
      {
        nome: "Triumph Street Triple",
        descricao: "Moto naked de alto desempenho e design agressivo.",
        detalhes: "Motor de 765cc, excelente para quem busca potência e agilidade.",
      },
      {
        nome: "Honda CB 1000R",
        descricao: "Uma moto naked com design moderno e motor potente.",
        detalhes: "Motor de 998cc, combina performance e conforto.",
      },
      {
        nome: "Royal Enfield Meteor 350",
        descricao: "Cruiser com estilo clássico e conforto.",
        detalhes: "Motor de 349cc, ideal para quem busca uma pilotagem tranquila.",
      }
    ];

    // Seleciona o container onde os cards das motos serão adicionados
    const catalogo = document.getElementById("motoCatalogo");

    // Cria os cards para cada moto e os adiciona ao DOM
    motos.forEach(moto => {
      const card = document.createElement("div");
      card.classList.add("moto-card");

      const titulo = document.createElement("h3");
      titulo.textContent = moto.nome;
      card.appendChild(titulo);

      const descricao = document.createElement("p");
      descricao.textContent = moto.descricao;
      card.appendChild(descricao);

      const detalhes = document.createElement("p");
      detalhes.classList.add("detalhes");
      detalhes.textContent = `Detalhes: ${moto.detalhes}`;
      card.appendChild(detalhes);

      const preco = document.createElement("p");
      preco.classList.add("preco");
      preco.textContent = `Preço: ${moto.preco}`;
      card.appendChild(preco);

      catalogo.appendChild(card);
    });
  </script>
</body>
</html>
