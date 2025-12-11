<!doctype html>
<html lang="pt-PT">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Cinq Lunes — Medidor de Anel</title>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="site-header">
    <div class="brand">
      <div class="moon">🌙</div>
      <div>
        <h1>Cinq Lunes</h1>
        <p class="tag">Elegância em todas as suas fases</p>
      </div>
    </div>
  </header>

  <main class="container">
    <section class="intro">
      <h2>Medidor de anel</h2>
      <p>Coloca o teu anel sobre o círculo para ver qual o tamanho aproximado. Antes de medir, calibra o ecrã com um cartão (85.6 mm).</p>
    </section>

    <section class="calibrator">
      <h3>1 — Calibrar ecrã</h3>
      <p>Coloca um cartão real (cartão de crédito = 85.6 mm) sobre o retângulo abaixo e ajusta o controlo até coincidir.</p>

      <div class="cal-box">
        <div class="card-marker" id="cardMarker"></div>
      </div>

      <div class="controls">
        <label for="pxPerMm">Escala: <span id="pxPerMmText">3.5</span> px/mm</label>
        <input id="pxPerMm" type="range" min="2" max="8" step="0.1" value="3.5">
        <button id="resetScale">Repor escala</button>
      </div>

      <p class="cal-tip">Dica: move o slider até o retângulo ter o mesmo comprimento do teu cartão. Guarda para uso futuro.</p>
    </section>

    <section class="sizer">
      <h3>2 — Medir o anel</h3>
      <p>Coloca o anel sobre o círculo central — ajusta o tamanho abaixo para encontrar o melhor encaixe.</p>

      <div class="sizer-area">
        <div id="ringCircle" class="ring-circle">
          <div id="circleLabel" class="circle-label">Coloca aqui o teu anel</div>
        </div>
      </div>

      <div class="size-controls">
        <label for="sizeSelect">Tamanho (PT):</label>
        <select id="sizeSelect"></select>

        <div class="size-info">
          <span>Diâmetro: <strong id="diamMM">—</strong> mm</span>
          <button id="downloadGuideline">Descarregar guia (PNG)</button>
        </div>
      </div>
    </section>

    <section class="table">
      <h3>Tabela de referência — anéis</h3>
      <p>Usa a tabela se preferires medir por diâmetro.</p>
      <pre class="size-table">
Tamanho — Diâmetro interno (mm)
10 — 16,0
11 — 16,5
12 — 17,0
13 — 17,2
14 — 17,8
15 — 18,5
16 — 19,0
17 — 19,3
18 — 19,7
19 — 20,4
20 — 21,0
      </pre>
    </section>

    <footer class="footer">
      <p>Cinq Lunes ✧ Prata 925 — Medidor de anel</p>
      <p>Link de referência: <a href="https://cinqlunes.com" target="_blank" rel="noopener">cinqlunes.com</a></p>
    </footer>
  </main>

  <script src="script.js"></script>
</body>
</html>
