<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Choose For Me</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0a0a0f;
    --surface: #13131a;
    --surface2: #1c1c28;
    --border: #2a2a3d;
    --accent: #f0c040;
    --accent2: #e05050;
    --accent3: #50c8e0;
    --text: #f0efe8;
    --muted: #8888a8;
    --radius: 14px;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    min-height: 100vh;
    overflow-x: hidden;
  }
  body::before {
    content: '';
    position: fixed; inset: 0;
    background-image:
      radial-gradient(1px 1px at 20% 30%, rgba(240,192,64,.4) 0%, transparent 100%),
      radial-gradient(1px 1px at 60% 70%, rgba(80,200,224,.3) 0%, transparent 100%),
      radial-gradient(1.5px 1.5px at 80% 20%, rgba(240,192,64,.2) 0%, transparent 100%),
      radial-gradient(1px 1px at 40% 85%, rgba(255,255,255,.15) 0%, transparent 100%),
      radial-gradient(1px 1px at 90% 50%, rgba(80,200,224,.2) 0%, transparent 100%);
    pointer-events: none; z-index: 0;
  }
  .app {
    position: relative; z-index: 1;
    max-width: 720px; margin: 0 auto;
    padding: 40px 24px 80px;
  }
  .header { text-align: center; margin-bottom: 48px; }
  .header h1 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(52px, 10vw, 88px);
    letter-spacing: 4px; line-height: 1;
    background: linear-gradient(135deg, var(--accent) 0%, #f08040 50%, var(--accent2) 100%);
    -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
  }
  .header p {
    color: var(--muted); font-size: 14px; letter-spacing: 2px;
    text-transform: uppercase; margin-top: 8px; font-weight: 500;
  }
  .card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: var(--radius);
    padding: 28px; margin-bottom: 20px;
    transition: border-color .2s, box-shadow .2s;
  }
  /* FIX 1: Required field error state */
  .card.error-required {
    border-color: var(--accent2) !important;
    box-shadow: 0 0 0 3px rgba(224,80,80,.18) !important;
    animation: shakeCard .38s ease;
  }
  @keyframes shakeCard {
    0%,100% { transform: translateX(0); }
    20% { transform: translateX(-7px); }
    40% { transform: translateX(7px); }
    60% { transform: translateX(-4px); }
    80% { transform: translateX(4px); }
  }
  .title-input.input-error {
    border-color: var(--accent2) !important;
    box-shadow: 0 0 0 3px rgba(224,80,80,.15) !important;
  }
  .error-hint {
    display: none; color: var(--accent2);
    font-size: 11px; letter-spacing: 1px;
    margin-top: 8px; font-family: 'DM Mono', monospace;
  }
  .error-hint.visible { display: block; }

  .section-label {
    font-family: 'DM Mono', monospace; font-size: 11px;
    letter-spacing: 3px; text-transform: uppercase;
    color: var(--accent); margin-bottom: 14px;
    display: flex; align-items: center; gap: 10px;
  }
  .section-label::after { content: ''; flex: 1; height: 1px; background: var(--border); }

  .title-input {
    width: 100%; background: var(--surface2);
    border: 1px solid var(--border); border-radius: 10px;
    padding: 16px 20px; font-family: 'DM Sans', sans-serif;
    font-size: 20px; font-weight: 500; color: var(--text);
    outline: none; transition: border-color .2s, box-shadow .2s;
  }
  .title-input::placeholder { color: var(--muted); }
  .title-input:focus { border-color: var(--accent); box-shadow: 0 0 0 3px rgba(240,192,64,.12); }

  .count-row { display: flex; gap: 12px; }
  .count-btn {
    flex: 1; padding: 18px 10px;
    background: var(--surface2); border: 1px solid var(--border);
    border-radius: 10px; color: var(--muted);
    font-family: 'Bebas Neue', sans-serif; font-size: 32px;
    letter-spacing: 2px; cursor: pointer; transition: all .2s;
  }
  .count-btn span {
    display: block; font-family: 'DM Sans', sans-serif;
    font-size: 9px; letter-spacing: 2px; text-transform: uppercase;
    margin-top: 2px; opacity: .6;
  }
  .count-btn:hover { border-color: var(--accent); color: var(--accent); transform: translateY(-1px); }
  .count-btn.active {
    background: rgba(240,192,64,.1); border-color: var(--accent);
    color: var(--accent); box-shadow: 0 0 20px rgba(240,192,64,.15);
  }

  .options-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; }
  .option-bubble {
    background: var(--surface2); border: 2px solid var(--border);
    border-radius: 100px; padding: 14px 22px;
    display: flex; align-items: center; gap: 10px;
    transition: border-color .2s, box-shadow .2s;
  }
  .option-bubble:focus-within { border-color: var(--accent3); box-shadow: 0 0 0 3px rgba(80,200,224,.1); }
  .option-num { font-family: 'Bebas Neue', sans-serif; font-size: 18px; color: var(--muted); min-width: 20px; }
  .option-input {
    background: none; border: none; outline: none;
    color: var(--text); font-family: 'DM Sans', sans-serif;
    font-size: 15px; font-weight: 500; width: 100%;
  }
  .option-input::placeholder { color: var(--muted); opacity: .6; }

  .cta-btn {
    width: 100%; padding: 20px;
    background: linear-gradient(135deg, var(--accent) 0%, #f08040 100%);
    border: none; border-radius: var(--radius);
    font-family: 'Bebas Neue', sans-serif; font-size: 26px;
    letter-spacing: 4px; color: #0a0a0f; cursor: pointer;
    transition: all .2s; margin-top: 8px;
  }
  .cta-btn:hover { transform: translateY(-2px); box-shadow: 0 12px 40px rgba(240,192,64,.3); }
  .cta-btn:active { transform: translateY(0); }

  /* ===== STAGE ===== */
  .stage-overlay {
    display: none; position: fixed; inset: 0;
    background: rgba(5,5,10,.93); backdrop-filter: blur(8px);
    z-index: 100; align-items: center; justify-content: center; flex-direction: column;
  }
  .stage-overlay.active { display: flex; }
  .stage-title {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(18px,4vw,28px); letter-spacing: 4px;
    color: var(--muted); margin-bottom: 10px;
    text-transform: uppercase; min-height: 36px; text-align: center;
  }
  .stage-question {
    font-size: clamp(14px,2.5vw,20px); font-weight: 600;
    color: var(--text); margin-bottom: 28px; text-align: center;
    max-width: 500px; padding: 0 20px;
  }
  .stage-arena {
    width: min(520px,92vw); height: 320px;
    position: relative; display: flex;
    align-items: center; justify-content: center;
  }

  /* ===== COIN — FIX 2 & 3: real coin SVG + animated flip ===== */
  .coin-scene { perspective: 700px; width: 160px; height: 160px; }
  .coin {
    width: 160px; height: 160px;
    position: relative; transform-style: preserve-3d; border-radius: 50%;
  }
  .coin.flipping { animation: coinToss 3s cubic-bezier(.25,.46,.45,.94) forwards; }
  @keyframes coinToss {
    0%   { transform: rotateY(0deg) translateY(0px); }
    15%  { transform: rotateY(540deg) translateY(-80px); }
    35%  { transform: rotateY(1260deg) translateY(-120px); }
    60%  { transform: rotateY(2160deg) translateY(-60px); }
    80%  { transform: rotateY(2880deg) translateY(-20px); }
    100% { transform: rotateY(var(--final-y,3240deg)) translateY(0px); }
  }
  .coin-face {
    position: absolute; inset: 0; border-radius: 50%;
    backface-visibility: hidden; overflow: hidden;
  }
  .coin-face.heads { transform: rotateY(0deg); }
  .coin-face.tails { transform: rotateY(180deg); }

  /* ===== BASEBALL HATS — FIX 4 ===== */
  .hat-scene { width: 100%; height: 100%; position: relative; }
  .hat-surface {
    position: absolute; bottom: 30px; left: 50%; transform: translateX(-50%);
    width: 400px; height: 6px;
    background: linear-gradient(90deg,#3a3020,#b0900a,#3a3020); border-radius: 3px;
  }
  .bhat {
    position: absolute; bottom: 36px;
    display: flex; flex-direction: column; align-items: center;
    width: 96px; cursor: default;
    transition: left .32s cubic-bezier(.4,0,.2,1), transform .7s cubic-bezier(.34,1.56,.64,1), filter .4s;
  }
  .bhat-name {
    font-family: 'DM Sans', sans-serif; font-size: 10px; font-weight: 600;
    color: var(--muted); margin-bottom: 4px; white-space: nowrap; text-align: center;
  }

  /* ===== BRACKET + LIGHTSABERS — FIX 5 ===== */
  .bracket-container { width: 100%; height: 100%; position: relative; }
  .bracket-svg { width: 100%; height: 100%; overflow: visible; }
  #saberCanvas { position: absolute; top: 0; left: 0; pointer-events: none; }

  /* ===== RESULT ===== */
  .result-reveal { display: none; text-align: center; margin-top: 20px; animation: fadeUp .5s ease forwards; }
  .result-reveal.show { display: block; }
  @keyframes fadeUp {
    from { opacity:0; transform:translateY(20px); }
    to   { opacity:1; transform:translateY(0); }
  }
  .result-label {
    font-family: 'DM Mono', monospace; font-size: 11px;
    letter-spacing: 3px; text-transform: uppercase;
    color: var(--muted); margin-bottom: 12px;
  }
  .result-choice {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(36px,8vw,64px); letter-spacing: 3px;
    background: linear-gradient(135deg,var(--accent) 0%,#f08040 100%);
    -webkit-background-clip: text; -webkit-text-fill-color: transparent;
    background-clip: text; margin-bottom: 24px;
  }
  .close-btn {
    padding: 12px 36px; background: transparent;
    border: 1px solid var(--border); border-radius: 100px;
    color: var(--muted); font-family: 'DM Mono', monospace;
    font-size: 12px; letter-spacing: 2px; text-transform: uppercase;
    cursor: pointer; transition: all .2s;
  }
  .close-btn:hover { border-color: var(--text); color: var(--text); }

  /* ===== HISTORY ===== */
  .history-section { margin-top: 8px; }
  .history-item {
    background: var(--surface2); border: 1px solid var(--border);
    border-radius: 10px; padding: 16px 20px; margin-bottom: 10px;
    display: flex; align-items: center; justify-content: space-between; gap: 16px;
  }
  .history-left { flex: 1; min-width: 0; }
  .history-q { font-size: 13px; font-weight: 500; color: var(--text); white-space: nowrap; overflow: hidden; text-overflow: ellipsis; margin-bottom: 4px; }
  .history-opts { font-size: 11px; color: var(--muted); font-family: 'DM Mono', monospace; }
  .history-right { text-align: right; flex-shrink: 0; }
  .history-answer { font-family: 'Bebas Neue', sans-serif; font-size: 22px; letter-spacing: 1px; color: var(--accent); }
  .history-time { font-size: 10px; color: var(--muted); font-family: 'DM Mono', monospace; margin-top: 2px; }
  .history-clear {
    background: none; border: none; color: var(--muted);
    font-family: 'DM Mono', monospace; font-size: 10px; letter-spacing: 1px;
    text-transform: uppercase; cursor: pointer; padding: 4px 8px;
    border-radius: 4px; transition: color .2s; margin-left: auto; display: block; margin-bottom: 10px;
  }
  .history-clear:hover { color: var(--accent2); }

  .confetti-piece {
    position: fixed; pointer-events: none; z-index: 200;
    animation: confettiFall linear forwards;
  }
  @keyframes confettiFall {
    0%   { transform: translateY(-20px) rotate(0deg); opacity: 1; }
    100% { transform: translateY(100vh) rotate(720deg); opacity: 0; }
  }
</style>
</head>
<body>
<div class="app">
  <div class="header">
    <h1>Choose For Me</h1>
    <p>When the mind can't decide, let fate intervene</p>
  </div>

  <!-- 01 Decision title -->
  <div class="card" id="titleCard">
    <div class="section-label">01 — What's the decision?</div>
    <input type="text" class="title-input" id="decisionTitle"
      placeholder="e.g. Where should we eat tonight?" maxlength="80">
    <div class="error-hint" id="titleError">⚠ Please enter your decision before continuing</div>
  </div>

  <!-- 02 Option count -->
  <div class="card">
    <div class="section-label">02 — How many options?</div>
    <div class="count-row">
      <button class="count-btn" data-count="2" onclick="selectCount(2)">2<span>coin flip</span></button>
      <button class="count-btn" data-count="3" onclick="selectCount(3)">3<span>hat game</span></button>
      <button class="count-btn" data-count="4" onclick="selectCount(4)">4<span>bracket</span></button>
    </div>
  </div>

  <!-- 03 Options -->
  <div class="card" id="optionsCard" style="display:none">
    <div class="section-label">03 — Enter your options</div>
    <div class="options-grid" id="optionsGrid"></div>
  </div>

  <button class="cta-btn" onclick="helpMeChoose()">Help Me Choose</button>

  <!-- History -->
  <div class="card history-section" id="historyCard" style="display:none">
    <div class="section-label">History</div>
    <button class="history-clear" onclick="clearHistory()">Clear all</button>
    <div id="historyList"></div>
  </div>
</div>

<!-- STAGE OVERLAY -->
<div class="stage-overlay" id="stageOverlay">
  <div class="stage-title" id="stageTitle">Deciding...</div>
  <div class="stage-question" id="stageQuestion"></div>
  <div class="stage-arena" id="stageArena"></div>
  <div class="result-reveal" id="resultReveal">
    <div class="result-label">The choice is clear</div>
    <div class="result-choice" id="resultChoice"></div>
    <button class="close-btn" onclick="closeStage()">Done</button>
  </div>
</div>

<script>
let selectedCount = 0;
let history = JSON.parse(localStorage.getItem('cfm_history') || '[]');

/* ---------- SETUP ---------- */
function selectCount(n) {
  selectedCount = n;
  document.querySelectorAll('.count-btn').forEach(b => b.classList.remove('active'));
  document.querySelector(`[data-count="${n}"]`).classList.add('active');
  buildOptionBubbles(n);
  document.getElementById('optionsCard').style.display = 'block';
}

function buildOptionBubbles(n) {
  const grid = document.getElementById('optionsGrid');
  grid.innerHTML = '';
  for (let i = 0; i < n; i++) {
    const d = document.createElement('div');
    d.className = 'option-bubble';
    d.innerHTML = `<span class="option-num">${String.fromCharCode(65+i)}</span>
      <input class="option-input" id="opt${i}" placeholder="Option ${String.fromCharCode(65+i)}" maxlength="30">`;
    grid.appendChild(d);
  }
}

// Clear error state when user types in title
document.getElementById('decisionTitle').addEventListener('input', () => {
  const v = document.getElementById('decisionTitle').value.trim();
  if (v) {
    document.getElementById('titleCard').classList.remove('error-required');
    document.getElementById('decisionTitle').classList.remove('input-error');
    document.getElementById('titleError').classList.remove('visible');
  }
});

/* ---------- MAIN TRIGGER ---------- */
function helpMeChoose() {
  const title = document.getElementById('decisionTitle').value.trim();

  // FIX 1: show red border if title missing
  if (!title) {
    const card = document.getElementById('titleCard');
    const inp  = document.getElementById('decisionTitle');
    const hint = document.getElementById('titleError');
    card.classList.remove('error-required');
    void card.offsetWidth; // restart animation
    card.classList.add('error-required');
    inp.classList.add('input-error');
    hint.classList.add('visible');
    inp.focus();
    return;
  }

  if (selectedCount < 2) {
    alert('Please select how many options you have (step 2).');
    return;
  }

  const options = [];
  for (let i = 0; i < selectedCount; i++) {
    const v = document.getElementById(`opt${i}`)?.value.trim();
    if (!v) { alert(`Please fill in Option ${String.fromCharCode(65+i)}`); return; }
    options.push(v);
  }

  const winner = options[Math.floor(Math.random() * options.length)];
  document.getElementById('stageQuestion').textContent = title;
  document.getElementById('resultReveal').classList.remove('show');
  document.getElementById('resultChoice').textContent = winner;
  document.getElementById('stageOverlay').classList.add('active');

  if      (selectedCount === 2) runCoinFlip(options, winner);
  else if (selectedCount === 3) runHatGame(options, winner);
  else                          runBracket(options, winner);

  history.unshift({
    title, options, winner,
    time: new Date().toLocaleString('en-US',{month:'short',day:'numeric',hour:'2-digit',minute:'2-digit'})
  });
  localStorage.setItem('cfm_history', JSON.stringify(history.slice(0,20)));
  renderHistory();
}

/* ================================================
   FIX 2 + 3 — COIN FLIP: real coin SVG + 3D flip
   ================================================ */
function makeCoinFaceSVG(label, side) {
  if (side === 'heads') {
    return `<svg viewBox="0 0 160 160" xmlns="http://www.w3.org/2000/svg" width="160" height="160">
      <defs>
        <radialGradient id="hg" cx="38%" cy="35%" r="60%">
          <stop offset="0%" stop-color="#fde988"/>
          <stop offset="55%" stop-color="#d4a017"/>
          <stop offset="100%" stop-color="#8a6200"/>
        </radialGradient>
      </defs>
      <circle cx="80" cy="80" r="78" fill="url(#hg)" stroke="#c8920a" stroke-width="4"/>
      <circle cx="80" cy="80" r="64" fill="none" stroke="rgba(255,220,80,.35)" stroke-width="2"/>
      <!-- Ridged edge marks -->
      ${Array.from({length:36},(_,i)=>{
        const a = (i/36)*Math.PI*2;
        const r1=73, r2=76;
        return `<line x1="${80+Math.cos(a)*r1}" y1="${80+Math.sin(a)*r1}" x2="${80+Math.cos(a)*r2}" y2="${80+Math.sin(a)*r2}" stroke="rgba(180,120,0,.5)" stroke-width="1"/>`;
      }).join('')}
      <!-- Portrait silhouette -->
      <ellipse cx="80" cy="60" rx="18" ry="22" fill="rgba(90,55,0,.55)"/>
      <path d="M55 92 Q80 76 105 92" fill="rgba(90,55,0,.4)" stroke="none"/>
      <!-- HEADS label -->
      <text x="80" y="116" font-family="Georgia,serif" font-size="13" letter-spacing="4" text-anchor="middle" fill="rgba(90,55,0,.9)">HEADS</text>
      <!-- Option -->
      <text x="80" y="134" font-family="'DM Sans',sans-serif" font-size="12" font-weight="700" text-anchor="middle" fill="rgba(90,55,0,.8)">${label}</text>
    </svg>`;
  } else {
    return `<svg viewBox="0 0 160 160" xmlns="http://www.w3.org/2000/svg" width="160" height="160">
      <defs>
        <radialGradient id="tg" cx="38%" cy="35%" r="60%">
          <stop offset="0%" stop-color="#e8e4dc"/>
          <stop offset="55%" stop-color="#9a9490"/>
          <stop offset="100%" stop-color="#5a5650"/>
        </radialGradient>
      </defs>
      <circle cx="80" cy="80" r="78" fill="url(#tg)" stroke="#8a8880" stroke-width="4"/>
      <circle cx="80" cy="80" r="64" fill="none" stroke="rgba(220,218,212,.4)" stroke-width="2"/>
      ${Array.from({length:36},(_,i)=>{
        const a = (i/36)*Math.PI*2;
        return `<line x1="${80+Math.cos(a)*73}" y1="${80+Math.sin(a)*73}" x2="${80+Math.cos(a)*76}" y2="${80+Math.sin(a)*76}" stroke="rgba(120,118,112,.5)" stroke-width="1"/>`;
      }).join('')}
      <!-- Eagle / shield motif -->
      <path d="M80 44 L90 60 L104 62 L94 73 L96 88 L80 80 L64 88 L66 73 L56 62 L70 60 Z" fill="rgba(40,36,30,.4)"/>
      <text x="80" y="116" font-family="Georgia,serif" font-size="13" letter-spacing="4" text-anchor="middle" fill="rgba(40,36,30,.85)">TAILS</text>
      <text x="80" y="134" font-family="'DM Sans',sans-serif" font-size="12" font-weight="700" text-anchor="middle" fill="rgba(40,36,30,.75)">${label}</text>
    </svg>`;
  }
}

function runCoinFlip(options, winner) {
  document.getElementById('stageTitle').textContent = 'Flipping the coin...';
  const arena = document.getElementById('stageArena');
  const headsWins = options.indexOf(winner) === 0;
  const spins = 9;
  const finalY = spins * 360 + (headsWins ? 0 : 180);

  arena.innerHTML = `
    <div class="coin-scene">
      <div class="coin" id="theCoin" style="--final-y:${finalY}deg">
        <div class="coin-face heads">${makeCoinFaceSVG(options[0],'heads')}</div>
        <div class="coin-face tails">${makeCoinFaceSVG(options[1],'tails')}</div>
      </div>
    </div>`;

  setTimeout(() => {
    document.getElementById('theCoin').classList.add('flipping');
    setTimeout(() => {
      document.getElementById('stageTitle').textContent = '🪙 The coin has spoken!';
      showResult();
    }, 3200);
  }, 150);
}

/* ================================================
   FIX 4 — HAT GAME: baseball caps + real swapping
   ================================================ */
function baseballCapSVG(fillColor, brimColor) {
  return `<svg width="90" height="72" viewBox="0 0 90 72" xmlns="http://www.w3.org/2000/svg">
    <!-- Brim -->
    <path d="M8 54 Q45 46 82 54 Q82 66 8 66 Z" fill="${brimColor}"/>
    <ellipse cx="45" cy="54" rx="38" ry="8" fill="${brimColor}"/>
    <!-- Crown -->
    <path d="M14 53 Q16 18 45 10 Q74 18 76 53 Z" fill="${fillColor}"/>
    <!-- Panel seams -->
    <path d="M45 10 Q38 30 36 53" stroke="rgba(0,0,0,.18)" stroke-width="1" fill="none"/>
    <path d="M45 10 Q52 30 54 53" stroke="rgba(0,0,0,.18)" stroke-width="1" fill="none"/>
    <!-- Highlight -->
    <path d="M24 50 Q28 24 45 14 Q50 22 48 36 Q44 33 38 36 Z" fill="rgba(255,255,255,.14)"/>
    <!-- Button -->
    <circle cx="45" cy="11" r="4.5" fill="${brimColor}" stroke="rgba(0,0,0,.2)" stroke-width="1"/>
    <!-- Sweatband -->
    <path d="M15 52 Q45 48 75 52" stroke="rgba(0,0,0,.22)" stroke-width="2" fill="none"/>
    <!-- Brim underside -->
    <path d="M10 56 Q45 50 80 56" stroke="rgba(0,0,0,.2)" stroke-width="1" fill="none"/>
  </svg>`;
}

function runHatGame(options, winner) {
  document.getElementById('stageTitle').textContent = 'Watch the hats...';
  const arena = document.getElementById('stageArena');

  const hatStyles = [
    { fill:'#1a4acc', brim:'#0f2888' },
    { fill:'#cc2020', brim:'#881010' },
    { fill:'#1a8833', brim:'#0f5522' },
  ];

  // Slot X positions (left edge of each 96px wide hat element)
  const slots = [20, 152, 284];

  arena.innerHTML = `<div class="hat-scene">
    <div class="hat-surface"></div>
    ${options.map((opt,i) => `
      <div class="bhat" id="bhat${i}" style="left:${slots[i]}px">
        <div class="bhat-name">${opt}</div>
        ${baseballCapSVG(hatStyles[i].fill, hatStyles[i].brim)}
      </div>`).join('')}
  </div>`;

  const winnerIdx = options.indexOf(winner);
  // Track current left-px positions for each hat by index
  let pos = [...slots];

  function moveHat(i, toX, dur) {
    const el = document.getElementById(`bhat${i}`);
    el.style.transitionDuration = dur + 'ms';
    el.style.left = toX + 'px';
    pos[i] = toX;
  }

  function swap(a, b, dur) {
    const pa = pos[a], pb = pos[b];
    moveHat(a, pb, dur);
    moveHat(b, pa, dur);
    return new Promise(r => setTimeout(r, dur + 60));
  }

  // Choreographed swap sequence (fast → slow)
  async function doShuffle() {
    const seq = [
      [[0,1],280], [[1,2],260], [[0,2],260],
      [[0,1],240], [[1,2],240], [[0,1],240],
      [[0,2],260], [[1,2],260], [[0,1],260],
      [[0,2],300], [[1,2],300],
      [[0,1],360], [[0,2],400],
      [[1,2],480],
    ];
    for (const [[a,b], dur] of seq) {
      await swap(a, b, dur);
    }
  }

  doShuffle().then(() => {
    setTimeout(() => {
      const winEl = document.getElementById(`bhat${winnerIdx}`);
      winEl.style.transitionDuration = '700ms';
      winEl.style.transform = 'translateY(-100px)';
      winEl.style.filter = `drop-shadow(0 0 16px ${hatStyles[winnerIdx].fill})`;
      document.getElementById('stageTitle').textContent = '🧢 There it is!';
      setTimeout(showResult, 900);
    }, 350);
  });
}

/* ================================================
   FIX 5 — BRACKET + LIGHTSABER FIGHTS
   ================================================ */
function runBracket(options, winner) {
  document.getElementById('stageTitle').textContent = 'The tournament begins!';
  const arena = document.getElementById('stageArena');

  const others = options.filter(o => o !== winner);
  for (let i = others.length-1; i>0; i--) {
    const j = Math.floor(Math.random()*(i+1));
    [others[i],others[j]] = [others[j],others[i]];
  }

  // Matchups
  const m1 = [winner, others[0]];         // winner always advances
  const m2 = [others[1], others[2]];
  const m2winner = Math.random()<.5 ? others[1] : others[2];

  // Saber colors for each combatant
  const c = {
    [m1[0]]: '#cc44ff',  // purple
    [m1[1]]: '#ff2222',  // red
    [m2[0]]: '#22ff55',  // green
    [m2[1]]: '#2288ff',  // blue
  };
  const finalC = { [winner]: '#22ff55', [m2winner]: '#ff2222' };

  arena.innerHTML = `<div class="bracket-container">
    <svg class="bracket-svg" id="bsvg" viewBox="0 0 500 300" xmlns="http://www.w3.org/2000/svg">
      <!-- Round 1 -->
      <rect x="6" y="28" width="140" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="rb0"/>
      <text x="76" y="51" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#f0efe8" id="rt0">${m1[0]}</text>
      <rect x="6" y="74" width="140" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="rb1"/>
      <text x="76" y="97" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#f0efe8" id="rt1">${m1[1]}</text>
      <rect x="6" y="162" width="140" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="rb2"/>
      <text x="76" y="185" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#f0efe8" id="rt2">${m2[0]}</text>
      <rect x="6" y="208" width="140" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="rb3"/>
      <text x="76" y="231" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#f0efe8" id="rt3">${m2[1]}</text>
      <!-- Connectors R1→Semi -->
      <path d="M146 45 H166 V91 H146" stroke="#2a2a3d" stroke-width="1.5" fill="none"/>
      <path d="M166 68 H184" stroke="#2a2a3d" stroke-width="1.5" fill="none" id="lc1"/>
      <path d="M146 179 H166 V225 H146" stroke="#2a2a3d" stroke-width="1.5" fill="none"/>
      <path d="M166 202 H184" stroke="#2a2a3d" stroke-width="1.5" fill="none" id="lc2"/>
      <!-- Semi boxes -->
      <rect x="184" y="51" width="140" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="sb1"/>
      <text x="254" y="74" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#444" id="st1">?</text>
      <rect x="184" y="185" width="140" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="sb2"/>
      <text x="254" y="208" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#444" id="st2">?</text>
      <!-- Connectors Semi→Final -->
      <path d="M324 68 H344 V202 H324" stroke="#2a2a3d" stroke-width="1.5" fill="none" id="lf"/>
      <path d="M344 135 H364" stroke="#2a2a3d" stroke-width="1.5" fill="none" id="lfb"/>
      <!-- Final box -->
      <rect x="364" y="118" width="128" height="34" rx="7" fill="#1c1c28" stroke="#2a2a3d" stroke-width="1.5" id="fb"/>
      <text x="428" y="141" text-anchor="middle" font-family="'DM Sans',sans-serif" font-size="11" font-weight="600" fill="#444" id="ft">?</text>
    </svg>
    <canvas id="saberCanvas"></canvas>
  </div>`;

  setTimeout(() => {
    const svgEl  = document.getElementById('bsvg');
    const canvas = document.getElementById('saberCanvas');
    const r = svgEl.getBoundingClientRect();
    canvas.width  = r.width;
    canvas.height = r.height;
    canvas.style.width  = r.width  + 'px';
    canvas.style.height = r.height + 'px';

    const sx = r.width / 500;
    const sy = r.height / 300;

    // Fight 1 — top half, center between m1 teams
    document.getElementById('stageTitle').textContent = 'Match 1 — Fight!';
    saberFight(canvas, sx*76, sy*68, c[m1[0]], c[m1[1]], 2400, () => {
      // Reveal m1 result
      document.getElementById('rt0').setAttribute('fill', m1[0]===winner ? '#f0c040' : '#555');
      document.getElementById('rt1').setAttribute('fill', m1[1]===winner ? '#f0c040' : '#555');
      document.getElementById('st1').textContent = winner;
      document.getElementById('st1').setAttribute('fill','#f0c040');
      document.getElementById('sb1').setAttribute('stroke','#f0c040');
      document.getElementById('lc1').setAttribute('stroke','#f0c040');

      // Fight 2 — bottom half
      setTimeout(() => {
        document.getElementById('stageTitle').textContent = 'Match 2 — Fight!';
        saberFight(canvas, sx*76, sy*202, c[m2[0]], c[m2[1]], 2400, () => {
          document.getElementById('rt2').setAttribute('fill', m2[0]===m2winner ? '#f0c040' : '#555');
          document.getElementById('rt3').setAttribute('fill', m2[1]===m2winner ? '#f0c040' : '#555');
          document.getElementById('st2').textContent = m2winner;
          document.getElementById('st2').setAttribute('fill','#f0c040');
          document.getElementById('sb2').setAttribute('stroke','#f0c040');
          document.getElementById('lc2').setAttribute('stroke','#f0c040');

          // Grand Final
          setTimeout(() => {
            document.getElementById('stageTitle').textContent = '⚔️ Grand Final — Fight!';
            saberFight(canvas, sx*254, sy*135, finalC[winner], finalC[m2winner], 3000, () => {
              document.getElementById('st1').setAttribute('fill','#888');
              document.getElementById('st2').setAttribute('fill','#888');
              document.getElementById('ft').textContent = winner;
              document.getElementById('ft').setAttribute('fill','#f0c040');
              document.getElementById('fb').setAttribute('stroke','#f0c040');
              document.getElementById('fb').setAttribute('fill','rgba(240,192,64,.1)');
              document.getElementById('lf').setAttribute('stroke','#f0c040');
              document.getElementById('lfb').setAttribute('stroke','#f0c040');
              document.getElementById('stageTitle').textContent = '🏆 Champion!';
              launchConfetti();
              setTimeout(showResult, 700);
            });
          }, 700);
        });
      }, 600);
    });
  }, 200);
}

/* Canvas lightsaber fight */
function saberFight(canvas, cx, cy, colorA, colorB, duration, onDone) {
  const ctx = canvas.getContext('2d');
  const t0  = performance.now();
  const len = Math.min(canvas.width, canvas.height) * 0.22;

  function glow(x1,y1,x2,y2,col,w) {
    ctx.save();
    ctx.shadowColor = col; ctx.shadowBlur = 20;
    ctx.strokeStyle = '#fff'; ctx.lineWidth = w*.35; ctx.lineCap='round';
    ctx.globalAlpha = .9;
    ctx.beginPath(); ctx.moveTo(x1,y1); ctx.lineTo(x2,y2); ctx.stroke();
    ctx.strokeStyle = col; ctx.lineWidth = w; ctx.globalAlpha = .8;
    ctx.beginPath(); ctx.moveTo(x1,y1); ctx.lineTo(x2,y2); ctx.stroke();
    ctx.restore();
  }

  function frame(now) {
    const elapsed = now - t0;
    const t = Math.min(elapsed/duration, 1);
    ctx.clearRect(0,0,canvas.width,canvas.height);

    const spd = 7 + t*4;
    const ph  = elapsed * 0.006 * spd;

    // Saber A: swings from left
    const aA = -0.4 + Math.sin(ph) * 0.7 + Math.cos(ph*0.6)*0.25;
    const ax2 = cx - 8 - Math.cos(aA)*len;
    const ay2 = cy     - Math.sin(aA)*len;
    glow(cx-8, cy, ax2, ay2, colorA, 3.5);

    // Saber B: swings from right
    const bA = Math.PI + 0.4 + Math.sin(ph+Math.PI)*0.7 + Math.cos(ph*0.6+1)*0.25;
    const bx2 = cx+8 - Math.cos(bA)*len;
    const by2 = cy   - Math.sin(bA)*len;
    glow(cx+8, cy, bx2, by2, colorB, 3.5);

    // Clash sparks
    const clash = Math.abs(Math.sin(ph*2.5));
    if (clash > 0.45) {
      const spkX = (ax2+bx2)/2, spkY=(ay2+by2)/2;
      for (let s=0; s<Math.floor(clash*8); s++) {
        const sa=Math.random()*Math.PI*2, sd=4+Math.random()*22;
        ctx.save();
        ctx.shadowColor='#fff'; ctx.shadowBlur=10;
        ctx.strokeStyle = Math.random()>.5 ? colorA : colorB;
        ctx.lineWidth=1.5; ctx.globalAlpha=clash*.85;
        ctx.beginPath();
        ctx.moveTo(spkX,spkY);
        ctx.lineTo(spkX+Math.cos(sa)*sd, spkY+Math.sin(sa)*sd);
        ctx.stroke(); ctx.restore();
      }
      // Flash orb
      ctx.save();
      ctx.globalAlpha = clash*.25;
      const g=ctx.createRadialGradient(spkX,spkY,0,spkX,spkY,24);
      g.addColorStop(0,'#ffffff'); g.addColorStop(1,'transparent');
      ctx.fillStyle=g;
      ctx.beginPath(); ctx.arc(spkX,spkY,24,0,Math.PI*2); ctx.fill();
      ctx.restore();
    }

    if (t < 1) requestAnimationFrame(frame);
    else { ctx.clearRect(0,0,canvas.width,canvas.height); if(onDone) onDone(); }
  }
  requestAnimationFrame(frame);
}

/* ---------- SHARED ---------- */
function showResult() {
  document.getElementById('resultReveal').classList.add('show');
  launchConfetti();
}
function launchConfetti() {
  const cols=['#f0c040','#e05050','#50c8e0','#80e050','#e050e0'];
  for(let i=0;i<55;i++){
    const c=document.createElement('div');
    c.className='confetti-piece';
    c.style.cssText=`left:${Math.random()*100}vw;background:${cols[Math.floor(Math.random()*cols.length)]};border-radius:${Math.random()>.5?'50%':'2px'};animation-duration:${1.5+Math.random()*2}s;animation-delay:${Math.random()*.5}s;width:${6+Math.random()*8}px;height:${6+Math.random()*8}px;`;
    document.body.appendChild(c);
    setTimeout(()=>c.remove(),4000);
  }
}
function closeStage() {
  document.getElementById('stageOverlay').classList.remove('active');
  document.getElementById('stageArena').innerHTML='';
}

/* ---------- HISTORY ---------- */
function renderHistory() {
  const card=document.getElementById('historyCard');
  const list=document.getElementById('historyList');
  if(!history.length){card.style.display='none';return;}
  card.style.display='block';
  list.innerHTML=history.map(h=>`
    <div class="history-item">
      <div class="history-left">
        <div class="history-q">${h.title}</div>
        <div class="history-opts">${h.options.join(' · ')}</div>
      </div>
      <div class="history-right">
        <div class="history-answer">${h.winner}</div>
        <div class="history-time">${h.time}</div>
      </div>
    </div>`).join('');
}
function clearHistory(){
  history=[];localStorage.removeItem('cfm_history');renderHistory();
}
renderHistory();
</script>
</body>
</html>
