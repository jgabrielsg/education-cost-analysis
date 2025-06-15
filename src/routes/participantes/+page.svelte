<script>
  const participants = [
    {
      name: 'Gustavo Bianchi',
      img: './images/gustavo.jpg',
      linkedin: 'https://www.linkedin.com/in/gustavobianchidasilva/',
      github: 'https://github.com/Gustyper'
    },
    {
      name: 'João Gabriel Machado',
      img: './images/eu.jpg',
      linkedin: 'https://www.linkedin.com/in/jo%C3%A3o-gabriel-machado-23b376218/',
      github: 'https://github.com/jgabrielsg'
    },
    {
      name: 'Vinicius Nascimento',
      img: './images/claudio.jpg',
      linkedin: 'https://www.linkedin.com/in/viniciuspnascimento/',
      github: 'http://github.com/Vinasque'
    }
  ];
</script>

<svelte:head>
  <title>Participantes</title>
</svelte:head>

<div class="container">
  {#each participants as p}
    <div class="card">
      <img class="photo" src={p.img} alt={p.name} />
      <div class="info">
        <h3>{p.name}</h3>
        <div class="links">
          <a href={p.linkedin} target="_blank" rel="noopener">
            <img class="icon" src="./images/linkedin.png" alt="LinkedIn" />
            LinkedIn
          </a>
          <a href={p.github} target="_blank" rel="noopener">
            <img class="icon" src="./images/github.png" alt="LinkedIn" />
             GitHub
          </a>
        </div>
      </div>
    </div>
  {/each}
</div>

<!-- Sobre Nós -->
<div class="about-us">
  <p>
    Olá! Somos estudantes de Ciência de Dados e Inteligência Artificial da FGV Rio (EMAP),
    e criamos este site para ajudar estudantes a encontrar a universidade ideal para eles,  
    combinando dados de custo de vida e qualidade de ensino, simplificando, ao menos
    um pouco, a difícil escolha de onde estudar no futuro.
  </p>
</div>

<!-- Referências -->
<h2 class="title">Referências</h2>
<ol class="references-list">
  <li>[1] Shamim, A. (2024). Cost of International Education [Data set]. Kaggle.</li>
  <li>[2] O’Neill, M. (2020). World University Rankings [Data set]. Kaggle.</li>
</ol>

<!-- Contatos -->
<div class="contact-section">
  <h3>Contatos</h3>
  <p>Para dúvidas ou sugestões, escreva para:</p>
  <ul class="contact-list">
    <li><a href="mailto:jogabriel433@gmail.com">jogabriel433@gmail.com</a></li>
    <li><a href="mailto:gu.bianchi.s@gmail.com">gu.bianchi.s@gmail.com</a></li>
    <li><a href="mailto:vinicius.nascimento05@hotmail.com">vinicius.nascimento05@hotmail.com</a></li>
  </ul>
</div>


<style>
  .container {
    display: flex;
    justify-content: space-around;
    align-items: flex-start;
    gap: 20px;
    padding: 20px;
  }

  .card {
    width: 240px;
    text-align: center;
    font-family: sans-serif;
  }

  .card img.photo {
    width: 240px;
    height: 200px;
    object-fit: cover;
    border-radius: 8px;
    transition: transform 0.3s, box-shadow 0.3s;
    cursor: pointer;
  }

  .card img.photo:hover {
    transform: scale(1.05);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
  }

  .info {
    margin-top: 8px;
  }

  .info h3 {
    margin: 8px 0 4px;
    font-size: 16px;
  }

  .links {
    display: flex;
    flex-direction: column;
    gap: 4px;
    font-size: 14px;
  }

  .links a {
    text-decoration: none;
    display: inline-flex;
    align-items: center;
    color: #0a66c2;
    transition: opacity 0.2s;
  }

  .links a:hover {
    opacity: 0.7;
  }

  .icon {
    width: 16px;
    height: 16px;
    margin-right: 6px;
  }

  .about-us {
    background: #03011e;
    padding: 16px 20px;
    border-left: 4px solid #0a66c2;
    border-radius: 4px;
    margin-bottom: 24px;
    font-size: 1rem;
    line-height: 1.5;
    color: #ffffff;
  }

  .title {
    font-size: 1.5rem;
    color: #222;
    margin: 32px 0 12px;
  }

  .references-list {
    margin: 0 0 24px 20px;
    color: #555;
  }
  .references-list li {
    margin-bottom: 8px;
  }

  .contact-section {
    background: #03011e;
    padding: 16px 20px;
    border-radius: 4px;
    font-size: 1rem;
    color: #ffffff;
  }
  .contact-section h3 {
    margin: 0 0 8px;
    font-size: 1.2rem;
  }
  .contact-section p {
    margin: 0 0 12px;
  }

  .contact-list {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .contact-list li {
    margin-bottom: 6px;
  }
  .contact-list a {
    color: #0a66c2;
    text-decoration: none;
    transition: opacity 0.2s;
  }
  .contact-list a:hover {
    opacity: 0.7;
  }
</style>