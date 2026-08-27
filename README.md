<!doctype html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Akey Koffi Clément — Géomètre-Topographe & Géographe SIG</title>
<meta name="description" content="Portfolio d'Akey Koffi Clément, opérateur géomètre-topographe et géographe SIG." />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Newsreader:ital,opsz,wght@0,6..72,400;0,6..72,500;1,6..72,400&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0D1321;
    --surface: #141B2E;
    --surface2: #0B0F1A;
    --accent: #C9A66B;
    --accent2: #5C8374;
    --text: #F1EDE4;
    --text-body: #c7cad6;
    --text-muted: #93A0B8;
    --nav-inactive: #5B6478;
    --border: rgba(201,166,107,0.16);
    --border-soft: rgba(255,255,255,0.06);
  }
  * { box-sizing: border-box; }
  html, body { margin:0; padding:0; min-height:100vh; background:var(--bg); }
  body {
    font-family: 'Newsreader', Georgia, serif;
    color: var(--text);
    -webkit-font-smoothing: antialiased;
  }
  .display { font-family: 'Space Grotesk', Arial, sans-serif; font-weight: 600; }
  .mono { font-family: 'JetBrains Mono', 'Courier New', monospace; }
  .serif { font-family: 'Newsreader', Georgia, serif; }

  .app { width:100%; min-height:100vh; display:flex; flex-direction:column; }

  .topbar { display:flex; align-items:center; gap:8px; padding:16px 24px; border-bottom:1px solid var(--border-soft); }
  .logo-mark { width:32px; height:32px; border-radius:8px; background:var(--accent); display:flex; align-items:center; justify-content:center; flex-shrink:0; }
  .brand { font-size:14px; letter-spacing:0.03em; }

  .tab-panel { display:none; flex:1; }
  .tab-panel.active { display:block; }

  .eyebrow { font-size:11px; letter-spacing:0.2em; text-transform:uppercase; color:var(--accent); display:flex; align-items:center; gap:8px; margin-bottom:12px; }
  .eyebrow .dash { width:16px; height:1px; background:var(--accent); display:inline-block; }

  .section { padding:40px 24px; }
  h1.hero-title { font-size:2.6rem; line-height:1.05; margin:0 0 12px; }
  h2.section-title { font-size:1.9rem; margin:0 0 24px; }

  .card { border-radius:16px; border:1px solid var(--border); background:var(--surface); padding:20px; box-shadow:0 8px 24px -12px rgba(0,0,0,0.5); }
  .card + .card { margin-top:16px; }
  .card.dashed { border-style:dashed; opacity:0.7; }

  .lede { color:var(--text-body); line-height:1.7; }
  .quote { font-family:'Newsreader',serif; font-style:italic; color:var(--accent2); text-align:center; margin:32px 16px; }

  .row { display:flex; align-items:center; justify-content:space-between; padding:12px 0; border-bottom:1px solid var(--border-soft); }
  .row:last-child { border-bottom:none; }
  .row .name { font-weight:500; }
  .row .sub { font-size:10px; color:var(--text-muted); text-transform:uppercase; letter-spacing:0.05em; }

  .chip { display:inline-block; padding:4px 12px; border-radius:999px; border:1px solid rgba(201,166,107,0.4); color:var(--text); font-size:12px; margin:4px 6px 0 0; }
  .tag { display:inline-block; padding:5px 10px; border-radius:6px; background:var(--bg); border:1px solid var(--border-soft); color:var(--text-muted); font-size:10px; margin:4px 6px 0 0; }

  .cert-item { display:flex; align-items:flex-start; gap:10px; margin-bottom:12px; }
  .cert-item svg { flex-shrink:0; margin-top:3px; }
  .cert-item span { color:var(--text-body); font-size:14px; }

  .btn-row { display:flex; flex-wrap:wrap; gap:12px; margin-top:28px; }
  .btn-primary { padding:12px 22px; border-radius:999px; background:var(--accent); color:var(--bg); font-weight:600; font-size:14px; border:none; text-decoration:none; display:inline-block; }
  .btn-outline { padding:12px 22px; border-radius:999px; border:1px solid rgba(201,166,107,0.5); color:var(--text); font-weight:600; font-size:14px; background:transparent; text-decoration:none; display:inline-block; }

  .contact-row { display:flex; align-items:center; gap:16px; padding:16px; border-radius:16px; border:1px solid var(--border); background:var(--surface); text-decoration:none; color:var(--text); margin-bottom:12px; }
  .contact-row svg { flex-shrink:0; }
  .contact-row .main { font-size:14px; font-weight:500; margin:0; }
  .contact-row .label { color:var(--text-muted); font-size:11px; margin:2px 0 0; font-family:'JetBrains Mono',monospace; }

  .hero { position:relative; min-height:65vh; display:flex; flex-direction:column; justify-content:center; overflow:hidden; }
  .hero-inner { position:relative; z-index:2; }
  .contour-svg { position:absolute; inset:0; width:100%; height:100%; opacity:0.16; pointer-events:none; }
  .contour-line { animation: drift 8s ease-in-out infinite; }
  @keyframes drift { 0%{transform:translateX(0)} 50%{transform:translateX(6px)} 100%{transform:translateX(0)} }
  @media (prefers-reduced-motion: reduce) { .contour-line { animation:none; } }

  .role { color:var(--text-muted); font-size:1.1rem; margin:0 0 2px; }
  .role2 { color:var(--accent2); font-style:italic; font-size:1.1rem; margin:0 0 20px; }

  .bottomnav { display:flex; border-top:1px solid var(--border-soft); background:var(--surface2); position:sticky; bottom:0; }
  .nav-btn { flex:1; display:flex; flex-direction:column; align-items:center; justify-content:center; gap:4px; padding:12px 0; background:none; border:none; cursor:pointer; }
  .nav-btn svg { color:var(--nav-inactive); }
  .nav-btn .label { font-size:10px; color:var(--nav-inactive); font-family:'JetBrains Mono',monospace; }
  .nav-btn.active svg, .nav-btn.active .label { color:var(--accent); }
</style>
</head>
<body>

<div class="app">

  <div class="topbar">
    <div class="logo-mark"><svg width="14" height="14" viewBox="0 0 24 24" fill="#0D1321"><path d="M12 3 2 21h20L12 3Z"/></svg></div>
    <span class="brand display">AKEY&nbsp;K.&nbsp;CLÉMENT</span>
  </div>

  <!-- ACCUEIL -->
  <div id="tab-accueil" class="tab-panel active">
    <div class="hero">
      <svg class="contour-svg" viewBox="0 0 400 500" preserveAspectRatio="xMidYMid slice">
        <ellipse cx="180" cy="60" rx="260" ry="40" fill="none" stroke="#C9A66B" stroke-width="1" class="contour-line" style="animation-delay:0s"/>
        <ellipse cx="220" cy="102" rx="254" ry="43" fill="none" stroke="#5C8374" stroke-width="1" class="contour-line" style="animation-delay:0.4s"/>
        <ellipse cx="180" cy="144" rx="248" ry="46" fill="none" stroke="#5C8374" stroke-width="1" class="contour-line" style="animation-delay:0.8s"/>
        <ellipse cx="220" cy="186" rx="242" ry="49" fill="none" stroke="#C9A66B" stroke-width="1" class="contour-line" style="animation-delay:1.2s"/>
        <ellipse cx="180" cy="228" rx="236" ry="52" fill="none" stroke="#5C8374" stroke-width="1" class="contour-line" style="animation-delay:1.6s"/>
        <ellipse cx="220" cy="270" rx="230" ry="55" fill="none" stroke="#5C8374" stroke-width="1" class="contour-line" style="animation-delay:2.0s"/>
        <ellipse cx="180" cy="312" rx="224" ry="58" fill="none" stroke="#C9A66B" stroke-width="1" class="contour-line" style="animation-delay:2.4s"/>
        <ellipse cx="220" cy="354" rx="218" ry="61" fill="none" stroke="#5C8374" stroke-width="1" class="contour-line" style="animation-delay:2.8s"/>
        <ellipse cx="180" cy="396" rx="212" ry="64" fill="none" stroke="#5C8374" stroke-width="1" class="contour-line" style="animation-delay:3.2s"/>
      </svg>
      <div class="hero-inner section">
        <div class="eyebrow"><span class="dash"></span>N 6.1319° · E 1.2228° — Agoè, Lomé</div>
        <h1 class="hero-title display">Akey Koffi<br>Clément</h1>
        <p class="role serif">Opérateur Géomètre-Topographe</p>
        <p class="role2 serif">&amp; Géographe SIG</p>
        <p class="lede" style="max-width:420px;">Du levé de terrain à la carte finie : analyse spatiale, SIG et topographie au service de l'aménagement du territoire.</p>
        <div class="btn-row">
          <button class="btn-primary" onclick="showTab('competences')">Voir les compétences</button>
          <button class="btn-outline" onclick="showTab('contact')">Me contacter</button>
        </div>
      </div>
    </div>
  </div>

  <!-- A PROPOS -->
  <div id="tab-apropos" class="tab-panel">
    <div class="section">
      <div class="eyebrow"><span class="dash"></span>Repère 002 — Profil</div>
      <h2 class="section-title display">À propos de moi</h2>

      <div class="card">
        <p class="lede">Opérateur géomètre-topographe et titulaire d'une licence en géographie, je dispose d'une solide familiarisation avec les Systèmes d'Information Géographique (SIG) et l'analyse spatiale. Habitué aux travaux de terrain, à la gestion du matériel de mesure et aux outils DAO/SIG (QGIS, AutoCAD), je souhaite intégrer une structure pour contribuer activement aux études topographiques et d'aménagement.</p>
      </div>

      <p class="quote">"L'innovation naît de la passion et de la persévérance."</p>

      <div class="eyebrow"><span class="dash"></span>Repère 003 — Parcours</div>
      <div class="card">
        <div style="display:flex; justify-content:space-between; align-items:flex-start;">
          <strong>Attestation d'Opérateur Topographe</strong>
          <span class="mono" style="font-size:10px; color:var(--accent); white-space:nowrap; margin-left:8px;">2025–2026</span>
        </div>
        <p style="color:var(--text-muted); font-size:14px; margin:4px 0 0;">Institut Formatec</p>
      </div>
      <div class="card">
        <div style="display:flex; justify-content:space-between; align-items:flex-start;">
          <strong>Licence Fondamentale en Géographie</strong>
          <span class="mono" style="font-size:10px; color:var(--accent); white-space:nowrap; margin-left:8px;">2021–2025</span>
        </div>
        <p style="color:var(--text-muted); font-size:14px; margin:4px 0 0;">Université de Lomé</p>
      </div>

      <div class="eyebrow" style="margin-top:32px;"><span class="dash"></span>Repère 004 — Certifications</div>
      <div class="cert-item"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374"><path d="M12 3 2 21h20L12 3Z"/></svg><span>Introduction à la gestion du cycle de projet</span></div>
      <div class="cert-item"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374"><path d="M12 3 2 21h20L12 3Z"/></svg><span>Suivi et évaluation d'un projet de développement (Groupe AFD)</span></div>
      <div class="cert-item"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374"><path d="M12 3 2 21h20L12 3Z"/></svg><span>Réseautage professionnel</span></div>
      <div class="cert-item"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374"><path d="M12 3 2 21h20L12 3Z"/></svg><span>Gestion de projet Agile</span></div>
      <div class="cert-item"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374"><path d="M12 3 2 21h20L12 3Z"/></svg><span>Site Web efficace</span></div>
    </div>
  </div>

  <!-- COMPETENCES -->
  <div id="tab-competences" class="tab-panel">
    <div class="section">
      <div class="eyebrow"><span class="dash"></span>Repère 010 — Boîte à outils</div>
      <h2 class="section-title display">Compétences</h2>

      <div class="card">
        <h3 class="mono" style="font-size:12px; text-transform:uppercase; letter-spacing:0.05em; color:var(--accent2); margin:0 0 8px;">Informatique &amp; SIG</h3>
        <div class="row"><span class="name">QGIS</span><span class="sub">Analyse spatiale</span></div>
        <div class="row"><span class="name">AutoCAD</span><span class="sub">DAO</span></div>
        <div class="row"><span class="name">KoboToolbox</span><span class="sub">Collecte numérique</span></div>
        <div class="row"><span class="name">Google Earth Pro</span><span class="sub">Cartographie</span></div>
      </div>

      <div class="card">
        <h3 class="mono" style="font-size:12px; text-transform:uppercase; letter-spacing:0.05em; color:var(--accent2); margin:0 0 8px;">Terrain &amp; gestion</h3>
        <div class="row"><span class="name">Topographie</span><span class="sub">Levé · Traitement · Implantation</span></div>
        <div class="row"><span class="name">Gestion de projet Agile</span></div>
        <div class="row"><span class="name">Suivi et évaluation</span></div>
      </div>

      <div class="card">
        <h3 class="mono" style="font-size:12px; text-transform:uppercase; letter-spacing:0.05em; color:var(--accent2); margin:0 0 8px;">Langues</h3>
        <div class="row"><span class="name">Français</span><span class="sub">Courant</span></div>
        <div class="row"><span class="name">Éwé</span><span class="sub">Courant</span></div>
        <div class="row"><span class="name">Anglais</span><span class="sub">Niveau scolaire</span></div>
      </div>

      <div class="card">
        <h3 class="mono" style="font-size:12px; text-transform:uppercase; letter-spacing:0.05em; color:var(--accent2); margin:0 0 8px;">Centres d'intérêt</h3>
        <span class="chip">Voyage</span><span class="chip">Technologie</span><span class="chip">Travail d'équipe</span>
      </div>
    </div>
  </div>

  <!-- PROJETS -->
  <div id="tab-projets" class="tab-panel">
    <div class="section">
      <div class="eyebrow"><span class="dash"></span>Repère 020 — Travaux</div>
      <h2 class="section-title display">Projets</h2>

      <div class="card">
        <div class="mono" style="font-size:10px; text-transform:uppercase; letter-spacing:0.05em; color:var(--accent); margin-bottom:8px;">Étude de cas SIG</div>
        <h3 style="margin:0 0 8px; font-size:1.15rem;">Cartographie des points d'eau (PMH)</h3>
        <p class="lede" style="font-size:14px;">Analyse spatiale sous QGIS pour identifier les villages prioritaires sans accès à l'eau au sein de limites préfectorales hexagonales : zones tampons, intersection spatiale, et automatisation du traitement via le Modeleur graphique (Graphical Modeler).</p>
        <div style="margin-top:8px;">
          <span class="tag">QGIS</span><span class="tag">Buffer</span><span class="tag">Intersection spatiale</span><span class="tag">Graphical Modeler</span>
        </div>
      </div>

      <div class="card dashed">
        <p style="color:var(--text-muted); font-size:14px; text-align:center; padding:16px 0; margin:0;">D'autres projets seront ajoutés prochainement — levés topographiques, implantations, missions terrain.</p>
      </div>
    </div>
  </div>

  <!-- CONTACT -->
  <div id="tab-contact" class="tab-panel">
    <div class="section">
      <div class="eyebrow"><span class="dash"></span>Repère 030 — Coordonnées</div>
      <h2 class="section-title display">Contact</h2>

      <a href="tel:+22897257151" class="contact-row">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#C9A66B" stroke-width="2"><path d="M6 3h3l2 5-2 1a11 11 0 0 0 6 6l1-2 5 2v3a2 2 0 0 1-2 2A16 16 0 0 1 4 5a2 2 0 0 1 2-2Z"/></svg>
        <div><p class="main">97 25 71 51 / 70 02 80 63</p><p class="label">Téléphone</p></div>
      </a>
      <a href="mailto:clementakey@gmail.com" class="contact-row">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#C9A66B" stroke-width="2"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="m4 7 8 6 8-6"/></svg>
        <div><p class="main">clementakey@gmail.com</p><p class="label">Email</p></div>
      </a>
      <div class="contact-row" style="cursor:default;">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#C9A66B" stroke-width="2"><path d="M12 21s7-6.6 7-12a7 7 0 1 0-14 0c0 5.4 7 12 7 12Z"/><circle cx="12" cy="9" r="2.5"/></svg>
        <div><p class="main">Agoè Plateau, Lomé — Togo</p><p class="label">Localisation</p></div>
      </div>

      <p class="quote" style="font-size:14px; margin-top:40px;">Disponible pour missions topographiques &amp; études SIG</p>
    </div>
  </div>

  <div class="bottomnav">
    <button class="nav-btn active" data-tab="accueil" onclick="showTab('accueil')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 9.5 12 3l9 6.5"/><path d="M5 10v10h14V10"/></svg>
      <span class="label">Accueil</span>
    </button>
    <button class="nav-btn" data-tab="apropos" onclick="showTab('apropos')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4.4 3.6-8 8-8s8 3.6 8 8"/></svg>
      <span class="label">À propos</span>
    </button>
    <button class="nav-btn" data-tab="competences" onclick="showTab('competences')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"/><path d="m15 9-3 3-3 3 3-3 3-3"/></svg>
      <span class="label">Compétences</span>
    </button>
    <button class="nav-btn" data-tab="projets" onclick="showTab('projets')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 4 3 6v14l6-2 6 2 6-2V4l-6 2-6-2Z"/><path d="M9 4v14M15 6v14"/></svg>
      <span class="label">Projets</span>
    </button>
    <button class="nav-btn" data-tab="contact" onclick="showTab('contact')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="m4 7 8 6 8-6"/></svg>
      <span class="label">Contact</span>
    </button>
  </div>

</div>

<script>
  function showTab(name) {
    document.querySelectorAll('.tab-panel').forEach(function(el){ el.classList.remove('active'); });
    document.getElementById('tab-' + name).classList.add('active');
    document.querySelectorAll('.nav-btn').forEach(function(btn){
      if (btn.getAttribute('data-tab') === name) { btn.classList.add('active'); }
      else { btn.classList.remove('active'); }
    });
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
</script>

</body>
</html>
