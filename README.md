<!doctype html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Akey Koffi Clément — Géomètre-Topographe & Géographe SIG</title>
<meta name="description" content="Portfolio d'Akey Koffi Clément, opérateur géomètre-topographe et géographe SIG." />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Newsreader:ital,opsz,wght@0,6..72,400;0,6..72,500;1,6..72,400&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<style>
  html, body { margin:0; padding:0; min-height:100vh; background:#0D1321; }
  body { font-family:'Newsreader', serif; }
  .font-display { font-family:'Space Grotesk', sans-serif; font-weight:600; }
  .font-mono { font-family:'JetBrains Mono', monospace; }
  .font-serif { font-family:'Newsreader', serif; }
  .tab-panel { display:none; }
  .tab-panel.active { display:block; }
  .nav-btn svg { color:#5B6478; }
  .nav-btn span { color:#5B6478; }
  .nav-btn.active svg, .nav-btn.active span { color:#C9A66B; }
  @keyframes driftContour { 0%{transform:translateX(0)} 50%{transform:translateX(6px)} 100%{transform:translateX(0)} }
  .contour-line { animation: driftContour 8s ease-in-out infinite; }
  @media (prefers-reduced-motion: reduce) { .contour-line { animation:none; } }
</style>
</head>
<body class="text-[#F1EDE4]">

<div class="w-full min-h-screen bg-[#0D1321] flex flex-col">

  <!-- Top bar -->
  <div class="flex items-center gap-2 px-6 py-4 border-b border-[#ffffff0d]">
    <div class="w-8 h-8 rounded-lg bg-[#C9A66B] flex items-center justify-center">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="#0D1321"><path d="M12 3 2 21h20L12 3Z"/></svg>
    </div>
    <span class="font-display text-[#F1EDE4] text-sm tracking-wide">AKEY&nbsp;K.&nbsp;CLÉMENT</span>
  </div>

  <!-- ================= ACCUEIL ================= -->
  <div id="tab-accueil" class="tab-panel active flex-1">
    <div class="relative min-h-[70vh] flex flex-col justify-center px-6 py-10 overflow-hidden">
      <svg class="absolute inset-0 w-full h-full opacity-[0.16] pointer-events-none" viewBox="0 0 400 500" preserveAspectRatio="xMidYMid slice">
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
      <div class="relative z-10">
        <div class="font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3">
          <span class="w-4 h-px bg-[#C9A66B]"></span>N 6.1319° · E 1.2228° — Agoè, Lomé
        </div>
        <h1 class="font-display text-[2.6rem] leading-[1.05] text-[#F1EDE4] mb-3">Akey Koffi<br>Clément</h1>
        <p class="text-[#93A0B8] font-serif text-lg mb-1">Opérateur Géomètre-Topographe</p>
        <p class="text-[#5C8374] font-serif text-lg italic mb-6">&amp; Géographe SIG</p>
        <p class="text-[#c7cad6] leading-relaxed mb-8 max-w-md">
          Du levé de terrain à la carte finie : analyse spatiale, SIG et topographie au service de l'aménagement du territoire.
        </p>
        <div class="flex flex-wrap gap-3">
          <button onclick="showTab('competences')" class="px-5 py-3 rounded-full bg-[#C9A66B] text-[#0D1321] font-semibold text-sm">Voir les compétences</button>
          <button onclick="showTab('contact')" class="px-5 py-3 rounded-full border border-[#C9A66B60] text-[#F1EDE4] font-semibold text-sm">Me contacter</button>
        </div>
      </div>
    </div>
  </div>

  <!-- ================= À PROPOS ================= -->
  <div id="tab-apropos" class="tab-panel flex-1">
    <div class="px-6 py-10">
      <div class="font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3"><span class="w-4 h-px bg-[#C9A66B]"></span>Repère 002 — Profil</div>
      <h2 class="font-display text-3xl text-[#F1EDE4] mb-6">À propos de moi</h2>

      <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5 mb-4">
        <p class="text-[#c7cad6] leading-relaxed">
          Opérateur géomètre-topographe et titulaire d'une licence en géographie, je dispose d'une solide familiarisation
          avec les Systèmes d'Information Géographique (SIG) et l'analyse spatiale. Habitué aux travaux de terrain, à la
          gestion du matériel de mesure et aux outils DAO/SIG (QGIS, AutoCAD), je souhaite intégrer une structure pour
          contribuer activement aux études topographiques et d'aménagement.
        </p>
      </div>

      <p class="font-serif italic text-[#5C8374] text-center my-8 px-4">"L'innovation naît de la passion et de la persévérance."</p>

      <div class="font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3"><span class="w-4 h-px bg-[#C9A66B]"></span>Repère 003 — Parcours</div>
      <div class="space-y-4">
        <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5">
          <div class="flex justify-between items-start mb-1">
            <h3 class="text-[#F1EDE4] font-semibold">Attestation d'Opérateur Topographe</h3>
            <span class="font-mono text-[10px] text-[#C9A66B] whitespace-nowrap ml-2">2025–2026</span>
          </div>
          <p class="text-[#93A0B8] text-sm">Institut Formatec</p>
        </div>
        <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5">
          <div class="flex justify-between items-start mb-1">
            <h3 class="text-[#F1EDE4] font-semibold">Licence Fondamentale en Géographie</h3>
            <span class="font-mono text-[10px] text-[#C9A66B] whitespace-nowrap ml-2">2021–2025</span>
          </div>
          <p class="text-[#93A0B8] text-sm">Université de Lomé</p>
        </div>
      </div>

      <div class="mt-8 font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3"><span class="w-4 h-px bg-[#C9A66B]"></span>Repère 004 — Certifications</div>
      <div class="space-y-3">
        <div class="flex items-start gap-3"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374" class="mt-1 shrink-0"><path d="M12 3 2 21h20L12 3Z"/></svg><span class="text-[#c7cad6] text-sm">Introduction à la gestion du cycle de projet</span></div>
        <div class="flex items-start gap-3"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374" class="mt-1 shrink-0"><path d="M12 3 2 21h20L12 3Z"/></svg><span class="text-[#c7cad6] text-sm">Suivi et évaluation d'un projet de développement (Groupe AFD)</span></div>
        <div class="flex items-start gap-3"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374" class="mt-1 shrink-0"><path d="M12 3 2 21h20L12 3Z"/></svg><span class="text-[#c7cad6] text-sm">Réseautage professionnel</span></div>
        <div class="flex items-start gap-3"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374" class="mt-1 shrink-0"><path d="M12 3 2 21h20L12 3Z"/></svg><span class="text-[#c7cad6] text-sm">Gestion de projet Agile</span></div>
        <div class="flex items-start gap-3"><svg width="12" height="12" viewBox="0 0 24 24" fill="#5C8374" class="mt-1 shrink-0"><path d="M12 3 2 21h20L12 3Z"/></svg><span class="text-[#c7cad6] text-sm">Site Web efficace</span></div>
      </div>
    </div>
  </div>

  <!-- ================= COMPÉTENCES ================= -->
  <div id="tab-competences" class="tab-panel flex-1">
    <div class="px-6 py-10">
      <div class="font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3"><span class="w-4 h-px bg-[#C9A66B]"></span>Repère 010 — Boîte à outils</div>
      <h2 class="font-display text-3xl text-[#F1EDE4] mb-6">Compétences</h2>

      <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5 mb-4">
        <h3 class="font-mono text-xs uppercase tracking-wider text-[#5C8374] mb-2">Informatique &amp; SIG</h3>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">QGIS</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Analyse spatiale</span></div>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">AutoCAD</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">DAO</span></div>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">KoboToolbox</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Collecte numérique</span></div>
        <div class="flex items-center justify-between py-3"><span class="font-medium">Google Earth Pro</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Cartographie</span></div>
      </div>

      <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5 mb-4">
        <h3 class="font-mono text-xs uppercase tracking-wider text-[#5C8374] mb-2">Terrain &amp; gestion</h3>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">Topographie</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Levé · Traitement · Implantation</span></div>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">Gestion de projet Agile</span></div>
        <div class="flex items-center justify-between py-3"><span class="font-medium">Suivi et évaluation</span></div>
      </div>

      <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5 mb-4">
        <h3 class="font-mono text-xs uppercase tracking-wider text-[#5C8374] mb-2">Langues</h3>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">Français</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Courant</span></div>
        <div class="flex items-center justify-between py-3 border-b border-[#ffffff0f]"><span class="font-medium">Éwé</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Courant</span></div>
        <div class="flex items-center justify-between py-3"><span class="font-medium">Anglais</span><span class="font-mono text-[10px] text-[#93A0B8] uppercase">Niveau scolaire</span></div>
      </div>

      <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5">
        <h3 class="font-mono text-xs uppercase tracking-wider text-[#5C8374] mb-2">Centres d'intérêt</h3>
        <div class="flex flex-wrap gap-2 mt-2">
          <span class="px-3 py-1 rounded-full border border-[#C9A66B40] text-[#F1EDE4] text-xs font-mono">Voyage</span>
          <span class="px-3 py-1 rounded-full border border-[#C9A66B40] text-[#F1EDE4] text-xs font-mono">Technologie</span>
          <span class="px-3 py-1 rounded-full border border-[#C9A66B40] text-[#F1EDE4] text-xs font-mono">Travail d'équipe</span>
        </div>
      </div>
    </div>
  </div>

  <!-- ================= PROJETS ================= -->
  <div id="tab-projets" class="tab-panel flex-1">
    <div class="px-6 py-10">
      <div class="font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3"><span class="w-4 h-px bg-[#C9A66B]"></span>Repère 020 — Travaux</div>
      <h2 class="font-display text-3xl text-[#F1EDE4] mb-6">Projets</h2>

      <div class="rounded-2xl border border-[#C9A66B29] bg-[#141B2E] p-5 mb-4">
        <div class="flex items-center justify-between mb-2">
          <span class="font-mono text-[10px] uppercase tracking-wider text-[#C9A66B]">Étude de cas SIG</span>
        </div>
        <h3 class="text-[#F1EDE4] font-semibold text-lg mb-2">Cartographie des points d'eau (PMH)</h3>
        <p class="text-[#c7cad6] text-sm leading-relaxed mb-3">
          Analyse spatiale sous QGIS pour identifier les villages prioritaires sans accès à l'eau au sein de limites
          préfectorales hexagonales : zones tampons, intersection spatiale, et automatisation du traitement via le
          Modeleur graphique (Graphical Modeler).
        </p>
        <div class="flex flex-wrap gap-2">
          <span class="px-2.5 py-1 rounded-md bg-[#0D1321] border border-[#ffffff0f] text-[#93A0B8] text-[10px] font-mono">QGIS</span>
          <span class="px-2.5 py-1 rounded-md bg-[#0D1321] border border-[#ffffff0f] text-[#93A0B8] text-[10px] font-mono">Buffer</span>
          <span class="px-2.5 py-1 rounded-md bg-[#0D1321] border border-[#ffffff0f] text-[#93A0B8] text-[10px] font-mono">Intersection spatiale</span>
          <span class="px-2.5 py-1 rounded-md bg-[#0D1321] border border-[#ffffff0f] text-[#93A0B8] text-[10px] font-mono">Graphical Modeler</span>
        </div>
      </div>

      <div class="rounded-2xl border border-dashed border-[#C9A66B29] bg-[#141B2E] p-5 opacity-70">
        <p class="text-[#93A0B8] text-sm text-center py-4">D'autres projets seront ajoutés prochainement — levés topographiques, implantations, missions terrain.</p>
      </div>
    </div>
  </div>

  <!-- ================= CONTACT ================= -->
  <div id="tab-contact" class="tab-panel flex-1">
    <div class="px-6 py-10">
      <div class="font-mono text-[11px] tracking-[0.2em] uppercase text-[#C9A66B] flex items-center gap-2 mb-3"><span class="w-4 h-px bg-[#C9A66B]"></span>Repère 030 — Coordonnées</div>
      <h2 class="font-display text-3xl text-[#F1EDE4] mb-6">Contact</h2>
      <div class="space-y-3">
        <a href="tel:+22897257151" class="flex items-center gap-4 p-4 rounded-2xl border border-[#C9A66B29] bg-[#141B2E]">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#C9A66B" stroke-width="2"><path d="M6 3h3l2 5-2 1a11 11 0 0 0 6 6l1-2 5 2v3a2 2 0 0 1-2 2A16 16 0 0 1 4 5a2 2 0 0 1 2-2Z"/></svg>
          <div><p class="text-sm font-medium">97 25 71 51 / 70 02 80 63</p><p class="text-[#93A0B8] text-xs font-mono">Téléphone</p></div>
        </a>
        <a href="mailto:clementakey@gmail.com" class="flex items-center gap-4 p-4 rounded-2xl border border-[#C9A66B29] bg-[#141B2E]">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#C9A66B" stroke-width="2"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="m4 7 8 6 8-6"/></svg>
          <div><p class="text-sm font-medium">clementakey@gmail.com</p><p class="text-[#93A0B8] text-xs font-mono">Email</p></div>
        </a>
        <div class="flex items-center gap-4 p-4 rounded-2xl border border-[#C9A66B29] bg-[#141B2E]">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#C9A66B" stroke-width="2"><path d="M12 21s7-6.6 7-12a7 7 0 1 0-14 0c0 5.4 7 12 7 12Z"/><circle cx="12" cy="9" r="2.5"/></svg>
          <div><p class="text-sm font-medium">Agoè Plateau, Lomé — Togo</p><p class="text-[#93A0B8] text-xs font-mono">Localisation</p></div>
        </div>
      </div>
      <p class="text-center text-[#5C8374] font-serif italic text-sm mt-10">Disponible pour missions topographiques &amp; études SIG</p>
    </div>
  </div>

  <!-- ================= BOTTOM NAV ================= -->
  <div class="flex items-stretch border-t border-[#ffffff0d] bg-[#0B0F1A] sticky bottom-0">
    <button class="nav-btn active flex-1 flex flex-col items-center justify-center gap-1 py-3" data-tab="accueil" onclick="showTab('accueil')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 9.5 12 3l9 6.5"/><path d="M5 10v10h14V10"/></svg>
      <span class="text-[10px] font-mono">Accueil</span>
    </button>
    <button class="nav-btn flex-1 flex flex-col items-center justify-center gap-1 py-3" data-tab="apropos" onclick="showTab('apropos')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4.4 3.6-8 8-8s8 3.6 8 8"/></svg>
      <span class="text-[10px] font-mono">À propos</span>
    </button>
    <button class="nav-btn flex-1 flex flex-col items-center justify-center gap-1 py-3" data-tab="competences" onclick="showTab('competences')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="9"/><path d="m15 9-3 3-3 3 3-3 3-3"/></svg>
      <span class="text-[10px] font-mono">Compétences</span>
    </button>
    <button class="nav-btn flex-1 flex flex-col items-center justify-center gap-1 py-3" data-tab="projets" onclick="showTab('projets')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 4 3 6v14l6-2 6 2 6-2V4l-6 2-6-2Z"/><path d="M9 4v14M15 6v14"/></svg>
      <span class="text-[10px] font-mono">Projets</span>
    </button>
    <button class="nav-btn flex-1 flex flex-col items-center justify-center gap-1 py-3" data-tab="contact" onclick="showTab('contact')">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="m4 7 8 6 8-6"/></svg>
      <span class="text-[10px] font-mono">Contact</span>
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
