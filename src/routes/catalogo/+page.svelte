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
  </style>
</head>
<body>
  <h2>Catálogo de Motos</h2>

  <div class="catalogo" id="motoCatalogo"></div>

  <script>
    let motos = [
      {
        nome: "Honda CB 500X",
        descricao: "Uma moto de aventura com design robusto."
      },
      {
        nome: "Yamaha MT-03",
        descricao: "Moto naked com motor potente."
      },
      {
        nome: "Kawasaki Ninja 400",
        descricao: "Motocicleta esportiva com alto desempenho."
      },
      {
        nome: "Suzuki V-Strom 650",
        descricao: "Moto de aventura com excelente estabilidade."
      },
      {
        nome: "BMW G 310 R",
        descricao: "Naked compacta, ágil e com ótimo custo-benefício."
      },
      {
        nome: "Ducati Scrambler 800",
        descricao: "Design clássico e motor de alto desempenho."
      },
      {
        nome: "Harley-Davidson Iron 883",
        descricao: "Cruiser com motor potente e visual icônico."
      },
      {
        nome: "Triumph Street Triple",
        descricao: "Moto naked de alto desempenho e design agressivo."
      },
      {
        nome: "Honda CB 1000R",
        descricao: "Uma moto naked com design moderno e motor potente."
      },
      {
        nome: "Royal Enfield Meteor 350",
        descricao: "Cruiser com estilo clássico e conforto."
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

      catalogo.appendChild(card);
    });
  </script>
</body>
</html>
