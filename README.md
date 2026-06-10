<!-- ============================================================
     GAUTAM SUKHANI — github.com/gautam0222
     A README that actually has a soul.
     ============================================================ -->

<div align="center">

<!-- ═══════════════════════════════════════════════════
     SVG 1: THE MAIN HEADER — NEURAL NETWORK UNIVERSE
     ═══════════════════════════════════════════════════ -->

<svg width="900" height="380" viewBox="0 0 900 380" xmlns="http://www.w3.org/2000/svg">
<defs>
  <style>
    .star { animation: twinkle 3s infinite alternate; fill: #ffffff; }
    .star:nth-child(2n) { animation-duration: 2.1s; }
    .star:nth-child(3n) { animation-duration: 4.3s; }
    .star:nth-child(5n) { animation-duration: 1.7s; }
    @keyframes twinkle { 0%{opacity:0.1} 100%{opacity:0.9} }
    .node { animation: pulse 2.5s infinite alternate; }
    .node:nth-child(2n) { animation-duration: 3.1s; }
    .node:nth-child(3n) { animation-duration: 1.9s; }
    @keyframes pulse {
      0%  { r: 5; opacity: 0.6; }
      100%{ r: 8; opacity: 1.0; }
    }
    .conn { stroke-dasharray: 6 4; animation: dash 3s linear infinite; }
    @keyframes dash { to { stroke-dashoffset: -40; } }
    .ship { animation: float 5s ease-in-out infinite; }
    @keyframes float {
      0%,100% { transform: translateY(0px); }
      50%      { transform: translateY(-12px); }
    }
    .glow-text {
      font-family: 'Courier New', monospace;
      fill: #00ffcc;
      filter: drop-shadow(0 0 8px #00ffcc88);
    }
    .scan { animation: scanmove 6s linear infinite; opacity: 0.04; }
    @keyframes scanmove { from{transform:translateY(-380px)} to{transform:translateY(380px)} }
    .orbit-dot { animation: orbit 8s linear infinite; transform-origin: 680px 190px; }
    .orbit-dot2 { animation: orbit 13s linear infinite reverse; transform-origin: 680px 190px; }
    @keyframes orbit { from{transform:rotate(0deg)} to{transform:rotate(360deg)} }
    .fade-in { animation: fadein 2s ease-in forwards; opacity: 0; }
    @keyframes fadein { to { opacity: 1; } }
  </style>

  <!-- Deep space gradient background -->
  <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%"   stop-color="#020510"/>
    <stop offset="50%"  stop-color="#060d1f"/>
    <stop offset="100%" stop-color="#0a0418"/>
  </linearGradient>

  <!-- Glow filter for nodes -->
  <filter id="glow">
    <feGaussianBlur stdDeviation="3" result="blur"/>
    <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>

  <!-- Strong glow for name -->
  <filter id="textglow">
    <feGaussianBlur stdDeviation="6" result="blur"/>
    <feMerge><feMergeNode in="blur"/><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>
</defs>

<!-- ── Background ── -->
<rect width="900" height="380" fill="url(#bg)" rx="16"/>

<!-- ── Scanline overlay ── -->
<rect class="scan" width="900" height="4" fill="#00ffcc" y="0"/>

<!-- ── Stars ── -->
<circle class="star" cx="23"  cy="17"  r="1.2" opacity="0.7"/>
<circle class="star" cx="67"  cy="44"  r="0.8" opacity="0.5"/>
<circle class="star" cx="112" cy="8"   r="1.5" opacity="0.6"/>
<circle class="star" cx="180" cy="31"  r="0.9" opacity="0.8"/>
<circle class="star" cx="244" cy="19"  r="1.1" opacity="0.4"/>
<circle class="star" cx="320" cy="52"  r="0.7" opacity="0.7"/>
<circle class="star" cx="411" cy="14"  r="1.3" opacity="0.5"/>
<circle class="star" cx="503" cy="38"  r="0.9" opacity="0.9"/>
<circle class="star" cx="574" cy="9"   r="1.4" opacity="0.6"/>
<circle class="star" cx="638" cy="47"  r="0.6" opacity="0.5"/>
<circle class="star" cx="720" cy="22"  r="1.0" opacity="0.8"/>
<circle class="star" cx="799" cy="11"  r="1.2" opacity="0.4"/>
<circle class="star" cx="861" cy="39"  r="0.8" opacity="0.7"/>
<circle class="star" cx="45"  cy="120" r="1.0" opacity="0.3"/>
<circle class="star" cx="130" cy="98"  r="0.7" opacity="0.6"/>
<circle class="star" cx="210" cy="145" r="1.3" opacity="0.4"/>
<circle class="star" cx="380" cy="110" r="0.9" opacity="0.8"/>
<circle class="star" cx="450" cy="90"  r="1.1" opacity="0.5"/>
<circle class="star" cx="760" cy="100" r="0.8" opacity="0.6"/>
<circle class="star" cx="840" cy="130" r="1.2" opacity="0.3"/>
<circle class="star" cx="30"  cy="300" r="0.9" opacity="0.5"/>
<circle class="star" cx="100" cy="330" r="1.1" opacity="0.7"/>
<circle class="star" cx="190" cy="290" r="0.7" opacity="0.4"/>
<circle class="star" cx="830" cy="310" r="1.0" opacity="0.6"/>
<circle class="star" cx="870" cy="270" r="0.8" opacity="0.8"/>
<circle class="star" cx="55"  cy="360" r="1.3" opacity="0.3"/>
<circle class="star" cx="810" cy="355" r="0.9" opacity="0.5"/>

<!-- ═══════════════════════════════════
     NEURAL NETWORK — LEFT SIDE
     ═══════════════════════════════════ -->

<!-- Connection lines (animated dashes) -->
<line class="conn" x1="80"  y1="160" x2="150" y2="220" stroke="#00ffcc" stroke-width="0.8" opacity="0.4"/>
<line class="conn" x1="80"  y1="160" x2="155" y2="110" stroke="#00ffcc" stroke-width="0.8" opacity="0.4"/>
<line class="conn" x1="150" y1="220" x2="240" y2="190" stroke="#7c3aed" stroke-width="0.8" opacity="0.4"/>
<line class="conn" x1="155" y1="110" x2="240" y2="190" stroke="#7c3aed" stroke-width="0.8" opacity="0.4"/>
<line class="conn" x1="240" y1="190" x2="310" y2="150" stroke="#00ffcc" stroke-width="0.8" opacity="0.5"/>
<line class="conn" x1="240" y1="190" x2="310" y2="240" stroke="#00ffcc" stroke-width="0.8" opacity="0.5"/>
<line class="conn" x1="150" y1="220" x2="120" y2="290" stroke="#7c3aed" stroke-width="0.8" opacity="0.3"/>
<line class="conn" x1="80"  y1="160" x2="50"  y2="230" stroke="#00ffcc" stroke-width="0.8" opacity="0.3"/>
<line class="conn" x1="310" y1="150" x2="375" y2="190" stroke="#7c3aed" stroke-width="0.8" opacity="0.4"/>
<line class="conn" x1="310" y1="240" x2="375" y2="190" stroke="#00ffcc" stroke-width="0.8" opacity="0.4"/>

<!-- Nodes -->
<circle class="node" cx="80"  cy="160" r="6" fill="#00ffcc" filter="url(#glow)" opacity="0.9"/>
<circle class="node" cx="150" cy="220" r="5" fill="#7c3aed" filter="url(#glow)" opacity="0.8"/>
<circle class="node" cx="155" cy="110" r="5" fill="#00ffcc" filter="url(#glow)" opacity="0.7"/>
<circle class="node" cx="240" cy="190" r="8" fill="#ffffff" filter="url(#glow)" opacity="0.9"/>
<circle class="node" cx="310" cy="150" r="5" fill="#00ffcc" filter="url(#glow)" opacity="0.8"/>
<circle class="node" cx="310" cy="240" r="5" fill="#7c3aed" filter="url(#glow)" opacity="0.8"/>
<circle class="node" cx="375" cy="190" r="7" fill="#00ffcc" filter="url(#glow)" opacity="0.9"/>
<circle class="node" cx="50"  cy="230" r="4" fill="#7c3aed" filter="url(#glow)" opacity="0.6"/>
<circle class="node" cx="120" cy="290" r="4" fill="#00ffcc" filter="url(#glow)" opacity="0.6"/>

<!-- Small satellite labels near key nodes -->
<text x="244" y="185" font-size="7" fill="#ffffff" opacity="0.5" text-anchor="middle" font-family="monospace">RAG</text>
<text x="379" y="185" font-size="7" fill="#ffffff" opacity="0.5" text-anchor="middle" font-family="monospace">LLM</text>

<!-- ═══════════════════════════════════
     GIANT NAME — CENTER
     ═══════════════════════════════════ -->

<text
  x="450" y="175"
  font-family="'Courier New', monospace"
  font-size="88"
  font-weight="900"
  text-anchor="middle"
  letter-spacing="12"
  fill="none"
  stroke="#00ffcc"
  stroke-width="1.5"
  filter="url(#textglow)"
  opacity="0.92"
  class="fade-in"
>GAUTAM</text>

<text
  x="450" y="225"
  font-family="'Courier New', monospace"
  font-size="15"
  font-weight="400"
  text-anchor="middle"
  letter-spacing="8"
  fill="#7c3aed"
  filter="url(#textglow)"
  opacity="0.85"
>AI · ML · FULL STACK · BUILDER</text>

<!-- Horizontal rule lines flanking subtitle -->
<line x1="150" y1="225" x2="290" y2="225" stroke="#7c3aed" stroke-width="0.5" opacity="0.5"/>
<line x1="610" y1="225" x2="750" y2="225" stroke="#7c3aed" stroke-width="0.5" opacity="0.5"/>

<!-- ═══════════════════════════════════
     ORBITING PLANET SYSTEM — RIGHT
     ═══════════════════════════════════ -->

<!-- Orbit rings (static circles) -->
<circle cx="720" cy="200" r="55" fill="none" stroke="#00ffcc" stroke-width="0.4" opacity="0.2" stroke-dasharray="3 5"/>
<circle cx="720" cy="200" r="85" fill="none" stroke="#7c3aed" stroke-width="0.4" opacity="0.2" stroke-dasharray="2 6"/>

<!-- Center "planet" -->
<circle cx="720" cy="200" r="18" fill="#0a0418" stroke="#00ffcc" stroke-width="1.5" filter="url(#glow)"/>
<text x="720" y="204" font-size="9" fill="#00ffcc" text-anchor="middle" font-family="monospace" font-weight="700">GS</text>

<!-- Inner orbit dot (rotates around center) -->
<g class="orbit-dot">
  <circle cx="775" cy="200" r="7" fill="#00ffcc" filter="url(#glow)" opacity="0.9"/>
  <text x="775" y="203" font-size="5.5" fill="#020510" text-anchor="middle" font-family="monospace" font-weight="700">AI</text>
</g>

<!-- Outer orbit dot -->
<g class="orbit-dot2">
  <circle cx="805" cy="200" r="7" fill="#7c3aed" filter="url(#glow)" opacity="0.9"/>
  <text x="805" y="203" font-size="5" fill="#ffffff" text-anchor="middle" font-family="monospace" font-weight="700">ML</text>
</g>

<!-- ═══════════════════════════════════
     BOTTOM STATUS BAR
     ═══════════════════════════════════ -->
<rect x="0" y="345" width="900" height="35" fill="#00ffcc" opacity="0.04" rx="0"/>
<line x1="0" y1="345" x2="900" y2="345" stroke="#00ffcc" stroke-width="0.5" opacity="0.3"/>

<circle cx="30" cy="362" r="5" fill="#00ff88" opacity="0.8"/>
<text x="45" y="367" font-size="11" fill="#00ffcc" font-family="monospace" opacity="0.7">ONLINE</text>
<text x="120" y="367" font-size="11" fill="#7c3aed" font-family="monospace" opacity="0.7">▸ Ceinsys Tech AI — MEG-NXT dept</text>
<text x="480" y="367" font-size="11" fill="#00ffcc" font-family="monospace" opacity="0.5">60 hrs/week · Nagpur → Everywhere</text>
<text x="760" y="367" font-size="11" fill="#7c3aed" font-family="monospace" opacity="0.5">github.com/gautam0222</text>

</svg>

<!-- ═══════════════════════════════════════════════════════════
     THE THREE LINES THAT DESCRIBE GAUTAM
     (Not resume. Not story. Just truth.)
     ═══════════════════════════════════════════════════════════ -->

<br/>

```
  Tier-3 college.  Chrome extensions live.  IEEE paper published.  Hackathon won.
  Business-background kid who learned to build things and couldn't stop.
  Currently obsessed with making machines that understand context — not just text.
```

<br/>

<!-- ═══════════════════════════════════════════════════════════
     SVG 2: THE SKILLS SOLAR SYSTEM
     ═══════════════════════════════════════════════════════════ -->

<svg width="900" height="340" viewBox="0 0 900 340" xmlns="http://www.w3.org/2000/svg">
<defs>
  <style>
    .p1 { animation: orbit1 7s  linear infinite; transform-origin: 450px 170px; }
    .p2 { animation: orbit2 11s linear infinite; transform-origin: 450px 170px; }
    .p3 { animation: orbit3 16s linear infinite; transform-origin: 450px 170px; }
    .p4 { animation: orbit4 22s linear infinite; transform-origin: 450px 170px; }
    .p1r{ animation: orbit1 7s  linear infinite reverse; transform-origin: 450px 170px; }
    .p2r{ animation: orbit2 11s linear infinite reverse; transform-origin: 450px 170px; }
    .p3r{ animation: orbit3 16s linear infinite reverse; transform-origin: 450px 170px; }
    .p4r{ animation: orbit4 22s linear infinite reverse; transform-origin: 450px 170px; }
    @keyframes orbit1 { from{transform:rotate(0deg)}   to{transform:rotate(360deg)} }
    @keyframes orbit2 { from{transform:rotate(45deg)}  to{transform:rotate(405deg)} }
    @keyframes orbit3 { from{transform:rotate(120deg)} to{transform:rotate(480deg)} }
    @keyframes orbit4 { from{transform:rotate(200deg)} to{transform:rotate(560deg)} }
    .pl { font-family: 'Courier New',monospace; font-weight:700; text-anchor:middle; dominant-baseline:central; }
    .ring-label { font-family:'Courier New',monospace; font-size:9px; fill:#ffffff; opacity:0.25; }
    .sun-pulse { animation: sunpulse 2s infinite alternate; }
    @keyframes sunpulse { 0%{r:28} 100%{r:32} }
  </style>
  <filter id="pglow">
    <feGaussianBlur stdDeviation="4" result="b"/>
    <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>
  <radialGradient id="starbg" cx="50%" cy="50%" r="50%">
    <stop offset="0%"   stop-color="#0d0221"/>
    <stop offset="100%" stop-color="#020510"/>
  </radialGradient>
</defs>

<rect width="900" height="340" fill="url(#starbg)" rx="16"/>

<!-- Section title -->
<text x="450" y="30" font-size="11" fill="#00ffcc" text-anchor="middle" font-family="monospace" letter-spacing="4" opacity="0.6">◈  SKILLS  UNIVERSE  ◈</text>

<!-- Orbit rings -->
<circle cx="450" cy="170" r="55"  fill="none" stroke="#ffffff" stroke-width="0.4" opacity="0.12"/>
<circle cx="450" cy="170" r="90"  fill="none" stroke="#ffffff" stroke-width="0.4" opacity="0.10"/>
<circle cx="450" cy="170" r="130" fill="none" stroke="#ffffff" stroke-width="0.4" opacity="0.08"/>
<circle cx="450" cy="170" r="170" fill="none" stroke="#ffffff" stroke-width="0.4" opacity="0.06"/>

<!-- Ring labels -->
<text class="ring-label" x="507" y="119">lang</text>
<text class="ring-label" x="542" y="84">frameworks</text>
<text class="ring-label" x="582" y="46">databases</text>
<text class="ring-label" x="622" y="16">tools</text>

<!-- ── SUN — the core skill ── -->
<circle class="sun-pulse" cx="450" cy="170" r="30" fill="#00ffcc" opacity="0.15" filter="url(#pglow)"/>
<circle cx="450" cy="170" r="26" fill="#0a0418" stroke="#00ffcc" stroke-width="2" filter="url(#pglow)"/>
<text x="450" y="166" class="pl" font-size="8" fill="#00ffcc">PYTHON</text>
<text x="450" y="177" class="pl" font-size="7" fill="#00ffcc" opacity="0.7">+ AI/ML</text>

<!-- ── RING 1 (r=55) — Languages ── -->
<g class="p1">
  <circle cx="505" cy="170" r="16" fill="#1e1b4b" stroke="#7c3aed" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="505" y="170" class="pl" font-size="7" fill="#a78bfa">C/C++</text>
</g>
<g class="p1r">
  <circle cx="395" cy="170" r="16" fill="#1e1b4b" stroke="#7c3aed" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="395" y="170" class="pl" font-size="7" fill="#a78bfa">TypeScript</text>
</g>

<!-- ── RING 2 (r=90) — Frameworks ── -->
<g class="p2">
  <circle cx="540" cy="170" r="18" fill="#042c30" stroke="#00ffcc" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="540" y="169" class="pl" font-size="7" fill="#00ffcc">LangGraph</text>
</g>
<g class="p2r">
  <circle cx="360" cy="170" r="18" fill="#042c30" stroke="#00ffcc" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="360" y="170" class="pl" font-size="7" fill="#00ffcc">FastAPI</text>
</g>
<g class="p3">
  <circle cx="450" cy="80" r="18" fill="#042c30" stroke="#00ffcc" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="450" y="80" class="pl" font-size="7" fill="#00ffcc">Flutter</text>
</g>
<g class="p3r">
  <circle cx="450" cy="260" r="18" fill="#042c30" stroke="#00ffcc" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="450" y="260" class="pl" font-size="7" fill="#00ffcc">React</text>
</g>

<!-- ── RING 3 (r=130) — Databases ── -->
<g class="p3">
  <circle cx="580" cy="170" r="20" fill="#0c1f0c" stroke="#22c55e" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="580" y="170" class="pl" font-size="7" fill="#4ade80">PostgreSQL</text>
</g>
<g class="p2r">
  <circle cx="320" cy="170" r="20" fill="#0c1f0c" stroke="#22c55e" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="320" y="170" class="pl" font-size="7" fill="#4ade80">MongoDB</text>
</g>
<g class="p4">
  <circle cx="450" cy="40"  r="20" fill="#0c1f0c" stroke="#22c55e" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="450" y="40" class="pl" font-size="7" fill="#4ade80">Firebase</text>
</g>
<g class="p1r">
  <circle cx="450" cy="300" r="20" fill="#0c1f0c" stroke="#22c55e" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="450" y="300" class="pl" font-size="7" fill="#4ade80">SQLite</text>
</g>

<!-- ── RING 4 (r=170) — Tools ── -->
<g class="p4">
  <circle cx="620" cy="170" r="22" fill="#1c0a00" stroke="#f97316" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="620" y="170" class="pl" font-size="7" fill="#fb923c">AWS</text>
</g>
<g class="p3r">
  <circle cx="280" cy="170" r="22" fill="#1c0a00" stroke="#f97316" stroke-width="1.2" filter="url(#pglow)"/>
  <text x="280" y="170" class="pl" font-size="7" fill="#fb923c">Docker</text>
</g>
<g class="p2">
  <circle cx="450" cy="0"   r="0" fill="none"/><!-- placeholder -->
</g>
<g class="p1">
  <circle cx="820" cy="170" r="0" fill="none"/><!-- out of view, ok -->
</g>

<!-- ── Static corner labels (skills that don't orbit — they're everywhere) ── -->
<rect x="14" y="50"  width="90" height="22" rx="11" fill="#1a0a2e" stroke="#7c3aed" stroke-width="0.8"/>
<text x="59" y="65"  class="pl" font-size="8" fill="#a78bfa">TensorFlow</text>

<rect x="14" y="82"  width="90" height="22" rx="11" fill="#1a0a2e" stroke="#7c3aed" stroke-width="0.8"/>
<text x="59" y="97"  class="pl" font-size="8" fill="#a78bfa">Scikit-learn</text>

<rect x="14" y="114" width="90" height="22" rx="11" fill="#1a0a2e" stroke="#7c3aed" stroke-width="0.8"/>
<text x="59" y="129" class="pl" font-size="8" fill="#a78bfa">PySpark</text>

<rect x="14" y="146" width="90" height="22" rx="11" fill="#042c30" stroke="#00ffcc" stroke-width="0.8"/>
<text x="59" y="161" class="pl" font-size="8" fill="#00ffcc">Vector DB</text>

<rect x="14" y="178" width="90" height="22" rx="11" fill="#042c30" stroke="#00ffcc" stroke-width="0.8"/>
<text x="59" y="193" class="pl" font-size="8" fill="#00ffcc">RAG</text>

<rect x="14" y="210" width="90" height="22" rx="11" fill="#042c30" stroke="#00ffcc" stroke-width="0.8"/>
<text x="59" y="225" class="pl" font-size="8" fill="#00ffcc">LLMs</text>

<rect x="796" y="50"  width="90" height="22" rx="11" fill="#0c1f0c" stroke="#22c55e" stroke-width="0.8"/>
<text x="841" y="65"  class="pl" font-size="8" fill="#4ade80">ServiceNow</text>

<rect x="796" y="82"  width="90" height="22" rx="11" fill="#0c1f0c" stroke="#22c55e" stroke-width="0.8"/>
<text x="841" y="97"  class="pl" font-size="8" fill="#4ade80">Git</text>

<rect x="796" y="114" width="90" height="22" rx="11" fill="#1c0a00" stroke="#f97316" stroke-width="0.8"/>
<text x="841" y="129" class="pl" font-size="8" fill="#fb923c">PowerBI</text>

<rect x="796" y="146" width="90" height="22" rx="11" fill="#1c0a00" stroke="#f97316" stroke-width="0.8"/>
<text x="841" y="161" class="pl" font-size="8" fill="#fb923c">Figma</text>

<rect x="796" y="178" width="90" height="22" rx="11" fill="#1c0a00" stroke="#f97316" stroke-width="0.8"/>
<text x="841" y="193" class="pl" font-size="8" fill="#fb923c">Node.js</text>

<rect x="796" y="210" width="90" height="22" rx="11" fill="#1a0a2e" stroke="#7c3aed" stroke-width="0.8"/>
<text x="841" y="225" class="pl" font-size="8" fill="#a78bfa">Flask</text>

</svg>

<br/>

<!-- ═══════════════════════════════════════════════════════════
     SVG 3: TERMINAL — THINGS GAUTAM HAS ACTUALLY DONE
     ═══════════════════════════════════════════════════════════ -->

<svg width="900" height="320" viewBox="0 0 900 320" xmlns="http://www.w3.org/2000/svg">
<defs>
  <style>
    .cursor { animation: blink 1s step-end infinite; }
    @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0} }
    .cmd  { font-family:'Courier New',monospace; font-size:12px; fill:#00ffcc; }
    .out  { font-family:'Courier New',monospace; font-size:12px; fill:#e2e8f0; }
    .dim  { font-family:'Courier New',monospace; font-size:12px; fill:#64748b; }
    .acc  { font-family:'Courier New',monospace; font-size:12px; fill:#a78bfa; }
    .hi   { font-family:'Courier New',monospace; font-size:12px; fill:#4ade80; }
    .warn { font-family:'Courier New',monospace; font-size:12px; fill:#fb923c; }
    .line-appear { animation: appear 0.3s ease forwards; opacity:0; }
    .line-appear:nth-child(1)  { animation-delay: 0.0s; }
    .line-appear:nth-child(2)  { animation-delay: 0.2s; }
    .line-appear:nth-child(3)  { animation-delay: 0.4s; }
    .line-appear:nth-child(4)  { animation-delay: 0.6s; }
    .line-appear:nth-child(5)  { animation-delay: 0.8s; }
    .line-appear:nth-child(6)  { animation-delay: 1.0s; }
    .line-appear:nth-child(7)  { animation-delay: 1.2s; }
    .line-appear:nth-child(8)  { animation-delay: 1.4s; }
    .line-appear:nth-child(9)  { animation-delay: 1.6s; }
    .line-appear:nth-child(10) { animation-delay: 1.8s; }
    .line-appear:nth-child(11) { animation-delay: 2.0s; }
    .line-appear:nth-child(12) { animation-delay: 2.2s; }
    .line-appear:nth-child(13) { animation-delay: 2.4s; }
    .line-appear:nth-child(14) { animation-delay: 2.6s; }
    .line-appear:nth-child(15) { animation-delay: 2.8s; }
    .line-appear:nth-child(16) { animation-delay: 3.0s; }
    .line-appear:nth-child(17) { animation-delay: 3.2s; }
    .line-appear:nth-child(18) { animation-delay: 3.4s; }
    @keyframes appear { from{opacity:0;transform:translateX(-4px)} to{opacity:1;transform:translateX(0)} }
  </style>
</defs>

<!-- Terminal window -->
<rect width="900" height="320" fill="#09090b" rx="16" stroke="#1e1b4b" stroke-width="1"/>

<!-- Title bar -->
<rect width="900" height="36" fill="#18181b" rx="16"/>
<rect width="900" height="20" y="16" fill="#18181b"/>
<circle cx="24" cy="18" r="6" fill="#ef4444" opacity="0.8"/>
<circle cx="44" cy="18" r="6" fill="#eab308" opacity="0.8"/>
<circle cx="64" cy="18" r="6" fill="#22c55e" opacity="0.8"/>
<text x="450" y="22" font-family="monospace" font-size="11" fill="#71717a" text-anchor="middle">gautam@universe: ~/life</text>

<!-- Terminal content — lines animate in sequentially -->
<g transform="translate(28, 58)">

  <text class="cmd line-appear" y="0">$ cat achievements.log</text>

  <text class="hi line-appear" y="22">  ✦  Won hackathon with AI disaster planner — 2023</text>
  <text class="hi line-appear" y="40">  ✦  Published IEEE ML paper — 2024</text>
  <text class="hi line-appear" y="58">  ✦  ByteGuard + TraceIt live on Chrome &amp; Edge Store</text>
  <text class="hi line-appear" y="76">  ✦  WalletWarp on Play Store — solo built</text>
  <text class="hi line-appear" y="94">  ✦  2× Merit Scholarship winner</text>
  <text class="hi line-appear" y="112">  ✦  OSINT ops with Nagpur Police (yes, real ones)</text>

  <text class="cmd line-appear" y="138">$ ./current_mission.sh</text>

  <text class="acc line-appear" y="160">  ⟶  Building MEG-NXT @ Ceinsys Tech AI</text>
  <text class="acc line-appear" y="178">  ⟶  RAG pipeline, embedding retrieval, vector search</text>
  <text class="acc line-appear" y="196">  ⟶  Open Context — AI knowledge system (10k+ docs indexed)</text>

  <text class="cmd line-appear" y="222">$ echo $OPEN_TO</text>

  <text class="warn line-appear" y="244">  AI/ML roles  ·  Backend  ·  Full-Stack  ·  Research  ·  Unhinged side projects</text>

  <text class="dim line-appear" y="270">  "The compiler doesn't care where you went to college."</text>

  <text class="cmd line-appear" y="292">$ <tspan class="cursor">_</tspan></text>

</g>
</svg>

<br/><br/>

<!-- ═══════════════════════════════════════════════════════════
     CONNECT — MINIMAL, NO BADGE SPAM
     ═══════════════════════════════════════════════════════════ -->

**`→`** [`github`](https://github.com/gautam0222) &nbsp;·&nbsp; [`leetcode`](https://leetcode.com/u/EuzXnztXui/) &nbsp;·&nbsp; [`portfolio`](https://gautam-sukhani.aptifolio.app/) &nbsp;·&nbsp; [`linkedin`](https://linkedin.com/in/gautam-sukhani-7751ba1b9) &nbsp;·&nbsp; [`mail`](mailto:sukhanigautam2@gmail.com)

</div>
