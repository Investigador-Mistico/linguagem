
<html><head><base href="/" />
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Linguagem Místico - Dashboard</title>
<style>
:root {
  --primary: #2e1065;
  --secondary: #4c1d95;
  --accent: #7c3aed;
  --text: #e2e8f0;
  --bg: #0f172a;
  --card-bg: #1e293b;
}

body {
  font-family: 'Inter', system-ui, sans-serif;
  margin: 0;
  padding: 2rem;
  background: var(--bg);
  color: var(--text);
  line-height: 1.6;
}

.header {
  text-align: center;
  margin-bottom: 4rem;
}

.mystical-logo {
  width: 120px;
  height: 120px;
  margin-bottom: 1rem;
  animation: pulse 2s infinite;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  margin-bottom: 3rem;
}

.stat-card {
  background: var(--card-bg);
  padding: 2rem;
  border-radius: 1rem;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s;
}

.stat-card:hover {
  transform: translateY(-5px);
}

.feature-section {
  background: var(--card-bg);
  padding: 3rem;
  border-radius: 1rem;
  margin-bottom: 3rem;
}

.code-block {
  background: #1a1a1a;
  padding: 2rem;
  border-radius: 0.5rem;
  overflow-x: auto;
  font-family: 'Fira Code', monospace;
  margin: 2rem 0;
}

.keyword { color: #ff79c6; }
.string { color: #f1fa8c; }
.comment { color: #6272a4; }

.cta-button {
  display: inline-flex;
  align-items: center;
  background: var(--accent);
  color: white;
  padding: 1rem 2rem;
  border-radius: 0.5rem;
  text-decoration: none;
  transition: transform 0.3s;
  margin: 1rem;
}

.cta-button:hover {
  transform: translateY(-2px);
}

.grid-showcase {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.showcase-card {
  background: var(--card-bg);
  padding: 2rem;
  border-radius: 1rem;
  text-align: center;
}

.showcase-icon {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  color: var(--accent);
}

@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.05); }
  100% { transform: scale(1); }
}

@media (max-width: 768px) {
  body {
    padding: 1rem;
  }
  
  .stats-grid {
    grid-template-columns: 1fr;
  }
  
  .feature-section {
    padding: 1.5rem;
  }
}
</style>
</head>
<body>

<header class="header">
  <svg class="mystical-logo" viewBox="0 0 100 100">
    <defs>
      <linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#7c3aed;stop-opacity:1" />
        <stop offset="100%" style="stop-color:#4c1d95;stop-opacity:1" />
      </linearGradient>
    </defs>
    <circle cx="50" cy="50" r="45" fill="none" stroke="url(#grad)" stroke-width="2"/>
    <path d="M50 5 L50 95 M5 50 L95 50" stroke="url(#grad)" stroke-width="2"/>
    <circle cx="50" cy="50" r="10" fill="url(#grad)"/>
  </svg>
  <h1>Místico</h1>
  <p>A Nova Era do Desenvolvimento Web</p>
</header>

<div class="stats-grid">
  <div class="stat-card">
    <h3>Downloads</h3>
    <p>10.5k+ este mês</p>
  </div>
  <div class="stat-card">
    <h3>Contribuidores</h3>
    <p>150+ desenvolvedores</p>
  </div>
  <div class="stat-card">
    <h3>Versão Atual</h3>
    <p>v2.1.0</p>
  </div>
</div>

<div class="feature-section">
  <h2>Uma Linguagem Revolucionária</h2>
  <p>Místico combina o poder do HTML, CSS, JavaScript e elementos místicos em uma única ferramenta poderosa para desenvolvimento web moderno.</p>
  
  <div class="code-block">
    <pre><code><span class="keyword">@ritual</span> criarComponente {
  <span class="keyword">invocar</span> ElementoMistico {
    nome: <span class="string">"Portal"</span>,
    energia: <span class="keyword">Agua</span>,
    <span class="comment">// Configuração do portal</span>
    configuracoes: {
      nivelEnergia: 5,
      elementoBase: "html"
    }
  }
}</code></pre>
  </div>
</div>

<div class="grid-showcase">
  <div class="showcase-card">
    <div class="showcase-icon">⚡</div>
    <h3>Performance Otimizada</h3>
    <p>Renderização ultra-rápida e código eficiente</p>
  </div>
  <div class="showcase-card">
    <div class="showcase-icon">🛠️</div>
    <h3>Ferramentas Poderosas</h3>
    <p>Suite completa de desenvolvimento</p>
  </div>
  <div class="showcase-card">
    <div class="showcase-icon">🌐</div>
    <h3>Compatibilidade Total</h3>
    <p>Funciona em qualquer navegador moderno</p>
  </div>
</div>

<div style="text-align: center;">
  <a href="https://github.com/Investigador-Mistico" class="cta-button" target="_blank">
    <svg style="width:24px;height:24px;margin-right:8px" viewBox="0 0 24 24">
      <path fill="currentColor" d="M12,2A10,10 0 0,0 2,12C2,16.42 4.87,20.17 8.84,21.5C9.34,21.58 9.5,21.27 9.5,21C9.5,20.77 9.5,20.14 9.5,19.31C6.73,19.91 6.14,17.97 6.14,17.97C5.68,16.81 5.03,16.5 5.03,16.5C4.12,15.88 5.1,15.9 5.1,15.9C6.1,15.97 6.63,16.93 6.63,16.93C7.5,18.45 8.97,18 9.54,17.76C9.63,17.11 9.89,16.67 10.17,16.42C7.95,16.17 5.62,15.31 5.62,11.5C5.62,10.39 6,9.5 6.65,8.79C6.55,8.54 6.2,7.5 6.75,6.15C6.75,6.15 7.59,5.88 9.5,7.17C10.29,6.95 11.15,6.84 12,6.84C12.85,6.84 13.71,6.95 14.5,7.17C16.41,5.88 17.25,6.15 17.25,6.15C17.8,7.5 17.45,8.54 17.35,8.79C18,9.5 18.38,10.39 18.38,11.5C18.38,15.32 16.04,16.16 13.81,16.41C14.17,16.72 14.5,17.33 14.5,18.26C14.5,19.6 14.5,20.68 14.5,21C14.5,21.27 14.66,21.59 15.17,21.5C19.14,20.16 22,16.42 22,12A10,10 0 0,0 12,2Z" />
    </svg>
    Explore no GitHub
  </a>
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  // Animação para cards
  const cards = document.querySelectorAll('.stat-card, .showcase-card');
  cards.forEach(card => {
    card.addEventListener('mouseover', () => {
      card.style.transform = 'translateY(-5px)';
      card.style.transition = 'transform 0.3s ease';
    });
    card.addEventListener('mouseout', () => {
      card.style.transform = 'translateY(0)';
    });
  });
});
</script>

</body></html>
