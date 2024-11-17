<template>
    <section class="features" id="features">
      <h2>¿Qué hace Taxia?</h2>
      <p>Taxia analiza los puntos clave de tu pregunta y selecciona activamente las fuentes más relevantes para responder.</p>
      <div class="feature-list">
        <div class="feature-item">
          <i class="icon-calculator"></i>
          <h3>Normativa Vigente e Histórica</h3>
          <p>Leyes, códigos, reglamentos, etc. Taxia puede navegar en el amplio universo del derecho mexicano.</p>
        </div>
        <div class="feature-item">
          <i class="icon-compliance"></i>
          <h3>Doctrina y Artículos</h3>
          <p>Hemos seleccionado la doctrina y los artículos más relevantes y especializados.</p>
        </div>
        <div class="feature-item">
          <i class="icon-strategy"></i>
          <h3>Jurisprudencia y Otros</h3>
          <p>Taxia puede investigar y descubrir precedentes judiciales relevantes a tus necesidades.</p>
        </div>
      </div>
    </section>
  </template>
  
  <style scoped>
  .features {
    padding: 60px 20px;
    text-align: center;
    background-color: #000000;
    color: #efefef;
  }
  
  .features h2 {
    color: #efefef;
    font-size: 2.5em;
    margin-bottom: 10px;
  }
  
  .features p {
    color: #b0b0b0;
    font-size: 1.2em;
    margin-bottom: 50px;
  }
  
  .feature-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }
  
  .feature-item {
    background-color: #131313;
    border-radius: 12px;
    padding: 30px;
    margin: 15px;
    flex: 1 1 calc(33.333% - 30px);
    max-width: calc(33.333% - 30px);
    text-align: center;
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
    transition: transform 0.3s;
  }
  
  .feature-item:hover {
    transform: translateY(-10px);
  }
  
  .feature-item i {
    font-size: 3em;
    color: #0733f9;
    margin-bottom: 20px;
  }
  
  .feature-item h3 {
    color: #efefef;
    font-size: 1.5em;
    margin-bottom: 15px;
  }
  
  .feature-item p {
    color: #efefef;
    font-size: 1em;
    line-height: 1.5;
  }
  
  /* Responsive Styles */
  @media (max-width: 992px) {
    .feature-item {
      flex: 1 1 calc(45% - 30px);
      max-width: calc(45% - 30px);
    }
  }
  
  @media (max-width: 600px) {
    .feature-item {
      flex: 1 1 100%;
      max-width: 100%;
    }
  }
  </style>
  