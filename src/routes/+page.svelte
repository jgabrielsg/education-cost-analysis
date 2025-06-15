<script>
  // nada aqui
</script>

<svelte:head>
  <title>Education Analysis - Home</title>
</svelte:head>

<section class="home-container">
  <div class="welcome">
    <h1>Education Analysis</h1>
    <p class="subtitle">Site geral com todos os links para o trabalho</p>
    <a href="./video" class="start-button">Trailer do Projeto</a>
    <p class="main-text">
      Este projeto nasceu para ajudar estudantes a escolher a universidade ideal no exterior, 
      levando em conta tanto o custo total (mensalidade, visto e aluguel) quanto a qualidade acadêmica via rankings mundiais.
    </p>

    <p class="main-text">
      Reunimos dados de mais de 600 instituições em 71 países (Kaggle), convertendo todos os valores para dólares e 
      calculando o custo total por curso. Desenvolvemos uma aplicação SPA em Svelte.js com componentes interativos 
      (mapas, gráficos de dispersão, barras e boxplots) para explorar esses dados de forma intuitiva.
    </p>

    <p class="main-text">
      Com visualizações coordenadas, o usuário pode comparar custos por distância, filtrar por nível de curso e país, 
      e avaliar a correlação entre custo e prestígio. No nosso estudo de caso, vimos que os EUA têm custo médio bem mais 
      alto ($120k) que Europa ($65k) e Ásia (~$26k), refletindo também nos rankings.
    </p>

    <p class="main-text">
      Em resumo, entregamos uma narrativa guiada e um “sandbox” exploratório que simplifica a análise de desigualdades 
      na educação global. O sistema é leve, responsivo e permite que cada estudante descubra insights práticos para 
      planejar seus estudos fora do país.
    </p>

    <a href="https://pt.overleaf.com/project/684ed7a7f3911ef213df0dbe">Link para o Artigo</a>
  </div>
</section>

<style>
  .home-container {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 85vh;
    background: linear-gradient(135deg, #000337 0%, #191414 100%);
    color: white;
    text-align: center;
  }

  .welcome {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1rem 1rem;
  }

  h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  /* legenda maior */
  p.subtitle {
    font-size: 1.8rem;
    font-weight: 500;
    margin: 0;
    color: #f0f0f0;
  }

  /* texto principal menor */
  p.main-text {
    font-size: 0.8rem;
    max-width: 700px;
    line-height: 1.6;
    color: #ddd;
    text-align: left;
  }

  .start-button {
    margin-top: 0.4rem;
    margin-bottom: 0.4rem;
    padding: 0.5rem 2rem;
    background-color: #191414;
    color: #1DB954;
    border: 2px solid #1DB954;
    border-radius: 9999px;
    font-size: 1.2rem;
    transition: all 0.3s ease;
    text-decoration: none;
  }

  .start-button:hover {
    background-color: #1DB954;
    color: #191414;
  }
</style>
