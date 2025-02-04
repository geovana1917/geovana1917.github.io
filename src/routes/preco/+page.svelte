<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Preços das Motos</title>
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
</head>
<body>
  <h2>Preços das Motos</h2>

  <div class="precos" id="motoPrecos"></div>

  <script>
    let motos = [
      {
        nome: "Honda CB 500X",
        preco: "R$ 29.990,00"
      },
      {
        nome: "Yamaha MT-03",
        preco: "R$ 23.990,00"
      },
      {
        nome: "Kawasaki Ninja 400",
        preco: "R$ 28.990,00"
      },
      {
        nome: "Suzuki V-Strom 650",
        preco: "R$ 34.990,00"
      },
      {
        nome: "BMW G 310 R",
        preco: "R$ 21.900,00"
      },
      {
        nome: "Ducati Scrambler 800",
        preco: "R$ 43.990,00"
      },
      {
        nome: "Harley-Davidson Iron 883",
        preco: "R$ 39.900,00"
      },
      {
        nome: "Triumph Street Triple",
        preco: "R$ 43.500,00"
      },
      {
        nome: "Honda CB 1000R",
        preco: "R$ 53.990,00"
      },
      {
        nome: "Royal Enfield Meteor 350",
        preco: "R$ 19.990,00"
      }
    ];

    // Seleciona o container onde os cards de preços serão adicionados
    const precosContainer = document.getElementById("motoPrecos");

    // Cria os cards para cada moto e os adiciona ao DOM
    motos.forEach(moto => {
      const card = document.createElement("div");
      card.classList.add("preco-card");

      const titulo = document.createElement("h3");
      titulo.textContent = moto.nome;
      card.appendChild(titulo);

      const preco = document.createElement("p");
      preco.innerHTML = `<strong>Preço:</strong> ${moto.preco}`;
      card.appendChild(preco);

      precosContainer.appendChild(card);
    });
  </script>
</body>
</html>
