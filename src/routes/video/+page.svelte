<script>
  // Sem nada aqui
</script>

<svelte:head>
  <title>Vídeo</title>
</svelte:head>

<div class="wrapper">
  <div class="video-card">
    <iframe
      src="https://www.youtube.com/embed/qStq1zw5sgw"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
    ></iframe>
  </div>
</div>

<a href="https://gvmail-my.sharepoint.com/:v:/g/personal/b51986_fgv_edu_br/Ef-r3rgt2mBAupADFLeFp2EBvd0jWj5n9r3dExsMegGOLg?e=3abn7b">Vídeo extra de 5 minutos</a>
<style>
  /* centraliza vertical/horizontalmente e usa 100% da viewport */
  .wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    background: #0d0924;
  }

  /* card preto com sombra, arredondado, com vídeo 100% */
  .video-card {
    width: 90%;
    height: 90%;
    max-width: 1200px;
    max-height: 800px;
    background: #000;
    border-radius: 8px;
    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.3);
    overflow: hidden;
  }

  .video-card iframe {
    width: 100%;
    height: 100%;
    display: block;
  }
</style>
