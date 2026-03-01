<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Chinmay Aswale — GitHub Profile Preview</title>
<link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@300;400;500;700&family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0a0a0f;
    --surface: #0f0f1a;
    --card: #13131f;
    --border: #1e1e32;
    --border-bright: #2a2a45;
    --accent: #4f6ef7;
    --accent2: #7c3aed;
    --green: #10b981;
    --amber: #f59e0b;
    --text: #e2e8f0;
    --muted: #64748b;
    --dim: #334155;
    --mono: 'JetBrains Mono', monospace;
    --sans: 'Space Grotesk', sans-serif;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: var(--sans);
    min-height: 100vh;
    padding: 40px 20px;
  }

  .container {
    max-width: 860px;
    margin: 0 auto;
  }

  /* ── HERO ── */
  .hero {
    position: relative;
    padding: 48px 0 40px;
    border-bottom: 1px solid var(--border);
    overflow: hidden;
  }

  .hero-grid {
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(79,110,247,0.04) 1px, transparent 1px),
      linear-gradient(90deg, rgba(79,110,247,0.04) 1px, transparent 1px);
    background-size: 40px 40px;
  }

  .hero-glow {
    position: absolute;
    top: -60px; left: -60px;
    width: 300px; height: 300px;
    background: radial-gradient(circle, rgba(79,110,247,0.12) 0%, transparent 70%);
    pointer-events: none;
  }

  .hero-content { position: relative; z-index: 1; }

  .status-pill {
    display: inline-flex;
    align-items: center;
    gap: 7px;
    background: rgba(16,185,129,0.08);
    border: 1px solid rgba(16,185,129,0.2);
    border-radius: 100px;
    padding: 5px 14px;
    font-family: var(--mono);
    font-size: 11px;
    color: var(--green);
    margin-bottom: 20px;
    letter-spacing: 0.05em;
  }

  .pulse {
    width: 6px; height: 6px;
    background: var(--green);
    border-radius: 50%;
    animation: pulse 2s infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 1; transform: scale(1); }
    50% { opacity: 0.4; transform: scale(0.8); }
  }

  .name {
    font-size: 42px;
    font-weight: 700;
    letter-spacing: -0.02em;
    line-height: 1;
    margin-bottom: 8px;
    background: linear-gradient(135deg, #e2e8f0 0%, #94a3b8 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .tagline {
    font-family: var(--mono);
    font-size: 14px;
    color: var(--accent);
    margin-bottom: 20px;
    opacity: 0.9;
  }

  .tagline span { color: var(--muted); }

  .bio {
    font-size: 15px;
    color: #94a3b8;
    line-height: 1.7;
    max-width: 580px;
    margin-bottom: 28px;
  }

  .links {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }

  .link-chip {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 7px 14px;
    background: var(--card);
    border: 1px solid var(--border-bright);
    border-radius: 8px;
    font-family: var(--mono);
    font-size: 12px;
    color: var(--muted);
    text-decoration: none;
    transition: all 0.2s;
  }

  .link-chip:hover {
    border-color: var(--accent);
    color: var(--accent);
  }

  /* ── SECTION ── */
  .section { padding: 36px 0 0; }

  .section-label {
    font-family: var(--mono);
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 0.15em;
    text-transform: uppercase;
    margin-bottom: 16px;
    display: flex;
    align-items: center;
    gap: 10px;
  }

  .section-label::after {
    content: '';
    flex: 1;
    height: 1px;
    background: var(--border);
  }

  /* ── STACK BADGES ── */
  .stack-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-bottom: 8px;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    gap: 5px;
    padding: 5px 12px;
    border-radius: 6px;
    font-family: var(--mono);
    font-size: 12px;
    font-weight: 500;
    border: 1px solid transparent;
  }

  .badge.rust    { background: rgba(239,138,78,0.1); border-color: rgba(239,138,78,0.2); color: #ef8a4e; }
  .badge.cpp     { background: rgba(79,110,247,0.1); border-color: rgba(79,110,247,0.2); color: #4f6ef7; }
  .badge.python  { background: rgba(250,204,21,0.1); border-color: rgba(250,204,21,0.2); color: #facc15; }
  .badge.next    { background: rgba(226,232,240,0.07); border-color: rgba(226,232,240,0.15); color: #cbd5e1; }
  .badge.aws     { background: rgba(245,158,11,0.1); border-color: rgba(245,158,11,0.2); color: #f59e0b; }
  .badge.llm     { background: rgba(124,58,237,0.1); border-color: rgba(124,58,237,0.2); color: #a78bfa; }
  .badge.green   { background: rgba(16,185,129,0.1); border-color: rgba(16,185,129,0.2); color: #34d399; }

  /* ── PROJECT CARDS ── */
  .projects-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
  }

  .proj-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 20px;
    position: relative;
    overflow: hidden;
    transition: border-color 0.2s;
  }

  .proj-card:hover { border-color: var(--border-bright); }

  .proj-card.featured {
    grid-column: span 2;
    background: linear-gradient(135deg, rgba(79,110,247,0.06) 0%, rgba(124,58,237,0.04) 100%);
    border-color: rgba(79,110,247,0.25);
  }

  .proj-accent {
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 2px;
    background: linear-gradient(90deg, var(--accent), var(--accent2));
    border-radius: 12px 12px 0 0;
  }

  .proj-name {
    font-size: 14px;
    font-weight: 600;
    margin-bottom: 6px;
    color: var(--text);
  }

  .proj-desc {
    font-size: 12px;
    color: var(--muted);
    line-height: 1.6;
    margin-bottom: 14px;
  }

  .proj-metrics {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
    margin-bottom: 12px;
  }

  .metric {
    font-family: var(--mono);
    font-size: 11px;
    padding: 3px 8px;
    background: rgba(79,110,247,0.08);
    border: 1px solid rgba(79,110,247,0.15);
    border-radius: 4px;
    color: #818cf8;
  }

  .metric.green {
    background: rgba(16,185,129,0.08);
    border-color: rgba(16,185,129,0.15);
    color: var(--green);
  }

  .proj-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .tag {
    font-family: var(--mono);
    font-size: 10px;
    color: var(--dim);
    background: rgba(255,255,255,0.03);
    padding: 2px 7px;
    border-radius: 4px;
    border: 1px solid var(--border);
  }

  /* ── STATS ROW ── */
  .stats-row {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 12px;
    margin-top: 16px;
  }

  .stat-card {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 10px;
    padding: 16px;
    text-align: center;
  }

  .stat-num {
    font-family: var(--mono);
    font-size: 22px;
    font-weight: 700;
    color: var(--accent);
    display: block;
  }

  .stat-label {
    font-size: 11px;
    color: var(--muted);
    margin-top: 4px;
  }

  /* ── CURRENTLY ── */
  .currently {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 20px 24px;
    margin-top: 16px;
  }

  .currently-items {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-top: 12px;
  }

  .curr-item {
    display: flex;
    align-items: flex-start;
    gap: 10px;
    font-size: 13px;
    color: #94a3b8;
    line-height: 1.5;
  }

  .curr-icon {
    font-size: 14px;
    margin-top: 1px;
    flex-shrink: 0;
  }

  /* ── FOOTER ── */
  .footer {
    margin-top: 40px;
    padding-top: 24px;
    border-top: 1px solid var(--border);
    font-family: var(--mono);
    font-size: 11px;
    color: var(--dim);
    text-align: center;
  }

  /* ── GITHUB LABEL ── */
  .gh-label {
    display: inline-block;
    font-family: var(--mono);
    font-size: 10px;
    color: var(--muted);
    background: var(--surface);
    border: 1px solid var(--border);
    padding: 2px 8px;
    border-radius: 4px;
    margin-bottom: 40px;
    letter-spacing: 0.1em;
  }
</style>
</head>
<body>
<div class="container">
  <div class="gh-label">▸ GITHUB PROFILE README — PREVIEW</div>

  <!-- HERO -->
  <div class="hero">
    <div class="hero-grid"></div>
    <div class="hero-glow"></div>
    <div class="hero-content">
      <div class="status-pill">
        <div class="pulse"></div>
        Open to AI Infra & Quant internships · 2026
      </div>
      <h1 class="name">Chinmay Aswale</h1>
      <div class="tagline">
        <span>// </span>I build AI systems that treat their own outputs as untrusted.
      </div>
      <p class="bio">
        3rd year Computer Engineering student at SPPU, Pune.<br>
        I work at the intersection of <strong style="color:#e2e8f0">agentic AI architecture</strong>, <strong style="color:#e2e8f0">systems engineering</strong>, and <strong style="color:#e2e8f0">quantitative finance</strong>.<br>
        My engineering philosophy: constrain non-determinism, validate at every boundary, rollback on failure.
      </p>
      <div class="links">
        <a class="link-chip" href="#">🌐 chinmayaswale.com</a>
        <a class="link-chip" href="#">💼 linkedin</a>
        <a class="link-chip" href="#">📄 resume</a>
        <a class="link-chip" href="#">✉️ poly.chinmay@gmail.com</a>
      </div>
    </div>
  </div>

  <!-- STACK -->
  <div class="section">
    <div class="section-label">stack</div>
    <div class="stack-grid">
      <span class="badge rust">⬡ Rust</span>
      <span class="badge cpp">⬡ C++</span>
      <span class="badge python">⬡ Python</span>
      <span class="badge next">⬡ Next.js</span>
      <span class="badge aws">⬡ AWS</span>
    </div>
    <div class="stack-grid">
      <span class="badge llm">⬡ LLM Fine-tuning (LoRA / QLoRA)</span>
      <span class="badge llm">⬡ Agentic Pipelines</span>
      <span class="badge green">⬡ Lock-free Systems</span>
      <span class="badge green">⬡ Quant / RL</span>
    </div>
  </div>

  <!-- FEATURED PROJECTS -->
  <div class="section">
    <div class="section-label">pinned projects</div>
    <div class="projects-grid">

      <!-- Ghost.ai — featured -->
      <div class="proj-card featured">
        <div class="proj-accent"></div>
        <div class="proj-name">🔒 Ghost.ai — Hardened Agentic Video Editor</div>
        <div class="proj-desc">7-stage deterministic validation pipeline for LLM outputs. AppOrchestrator coordinates 9 independent engines — zero direct engine-to-engine calls. LLM outputs treated as untrusted until validated across all stages.</div>
        <div class="proj-metrics">
          <span class="metric green">0 unsafe state transitions</span>
          <span class="metric">13 production phases</span>
          <span class="metric">9 orchestrated engines</span>
          <span class="metric">Atomic rollback</span>
        </div>
        <div class="proj-tags">
          <span class="tag">Rust</span>
          <span class="tag">Python</span>
          <span class="tag">Tauri</span>
          <span class="tag">React</span>
          <span class="tag">LLM Pipeline</span>
          <span class="tag">Event Sourcing</span>
        </div>
      </div>

      <!-- Order Book -->
      <div class="proj-card">
        <div class="proj-name">⚡ Ultra-Low Latency Order Book Engine</div>
        <div class="proj-desc">Lock-free limit order book matching engine with custom memory pool allocators and deterministic replay.</div>
        <div class="proj-metrics">
          <span class="metric">Microsecond latency</span>
          <span class="metric green">vs naive STL benchmarked</span>
        </div>
        <div class="proj-tags">
          <span class="tag">C++</span>
          <span class="tag">Lock-free DS</span>
          <span class="tag">Memory Pools</span>
        </div>
      </div>

      <!-- LLaMA Fine-tune -->
      <div class="proj-card">
        <div class="proj-name">🧠 LLaMA-2-7B Supply Chain Fine-tune</div>
        <div class="proj-desc">LoRA fine-tune on 8,200 domain QA pairs. Deployed via AWS Lambda + API Gateway.</div>
        <div class="proj-metrics">
          <span class="metric green">61% → 84% accuracy</span>
          <span class="metric">22% latency ↓</span>
        </div>
        <div class="proj-tags">
          <span class="tag">Python</span>
          <span class="tag">LoRA r=8</span>
          <span class="tag">AWS Lambda</span>
        </div>
      </div>

      <!-- RL Market Maker -->
      <div class="proj-card">
        <div class="proj-name">📈 RL Market Maker</div>
        <div class="proj-desc">DQN agent learning optimal bid-ask spreads. 2.5M timesteps on 3 years of crypto tick data.</div>
        <div class="proj-metrics">
          <span class="metric green">Sharpe 0.8 → 1.9</span>
          <span class="metric">Drawdown ↓17%</span>
        </div>
        <div class="proj-tags">
          <span class="tag">Python</span>
          <span class="tag">DQN</span>
          <span class="tag">Custom LOB Sim</span>
        </div>
      </div>

    </div>
  </div>

  <!-- STATS -->
  <div class="section">
    <div class="section-label">by the numbers</div>
    <div class="stats-row">
      <div class="stat-card">
        <span class="stat-num">20+</span>
        <div class="stat-label">Projects Built</div>
      </div>
      <div class="stat-card">
        <span class="stat-num">3</span>
        <div class="stat-label">LLMs Fine-tuned</div>
      </div>
      <div class="stat-card">
        <span class="stat-num">1.9</span>
        <div class="stat-label">Best Sharpe Ratio</div>
      </div>
      <div class="stat-card">
        <span class="stat-num">3+</span>
        <div class="stat-label">Production Sites</div>
      </div>
    </div>
  </div>

  <!-- CURRENTLY -->
  <div class="section">
    <div class="section-label">currently</div>
    <div class="currently">
      <div class="currently-items">
        <div class="curr-item"><span class="curr-icon">🔨</span> Building Ghost.ai — AI-integrated video editor with hardened agentic pipeline in Rust</div>
        <div class="curr-item"><span class="curr-icon">📖</span> Preparing for CFA Level 1 — August 2026</div>
        <div class="curr-item"><span class="curr-icon">🎯</span> Targeting AI infrastructure & quant internships for 2026</div>
        <div class="curr-item"><span class="curr-icon">🌐</span> Running DPMUN 2026 — conference management platform at dpmun.in</div>
      </div>
    </div>
  </div>

  <div class="footer">
    &ldquo;The LLM never touches application state directly.&rdquo; &mdash; ghost.ai architecture doc
  </div>

</div>
</body>
</html>
