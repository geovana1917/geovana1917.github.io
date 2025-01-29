<script>
  let motos = [
    {
      nome: "Honda CB 500X",
      descricao: "Uma moto de aventura com design robusto."
    },
    {
      nome: "Yamaha MT-03",
      descricao: "Moto naked com motor potente."
    }
  ];
</script>

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

<h2>Catálogo de Motos</h2>

<div class="catalogo">
  {#each motos as moto}
    <div class="moto-card">
      <h3>{moto.nome}</h3>
      <p>{moto.descricao}</p>
    </div>
  {/each}
</div>
