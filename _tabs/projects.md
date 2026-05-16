---
layout: page
title: Projects
icon: fas fa-code
order: 2
---

A collection of apps and tools I've built — covering personal finance, cybersecurity, algorithmic trading, and client web work. Everything runs locally or in the browser, no proprietary cloud required.

---

<style>
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
}
.project-card {
  border: 1px solid var(--border-color, rgba(255,255,255,0.1));
  border-radius: 12px;
  overflow: hidden;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  background: var(--card-bg, #1a1a2e);
  text-decoration: none !important;
  display: block;
  color: inherit;
}
.project-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 12px 32px rgba(0,0,0,0.3);
  text-decoration: none !important;
}
.project-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  object-position: top;
  display: block;
  border-bottom: 1px solid var(--border-color, rgba(255,255,255,0.08));
}
.project-card-body {
  padding: 1rem 1.1rem 1.1rem;
}
.project-card-title {
  font-size: 0.95rem;
  font-weight: 700;
  margin: 0 0 0.35rem;
  color: var(--heading-color, #f0f0f0);
}
.project-card-desc {
  font-size: 0.8rem;
  color: var(--text-muted-color, #888);
  margin: 0 0 0.75rem;
  line-height: 1.5;
}
.project-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.35rem;
}
.project-tag {
  font-size: 0.68rem;
  font-weight: 600;
  padding: 0.2rem 0.55rem;
  border-radius: 99px;
  background: rgba(99,102,241,0.15);
  color: #818cf8;
  letter-spacing: 0.02em;
}
</style>

<div class="project-grid">

  <a class="project-card" href="/posts/building-budget-coach-a-mobile-first-personal-finance-app/">
    <img src="/assets/img/projects/budget-coach.png" alt="Budget Coach" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">Budget Coach</p>
      <p class="project-card-desc">Mobile-first personal finance app — Safe-to-Spend calculator, bills, subscriptions, debt payoff, savings goals, couples mode. 100% local, no backend.</p>
      <div class="project-tags">
        <span class="project-tag">React</span>
        <span class="project-tag">TypeScript</span>
        <span class="project-tag">Tailwind</span>
        <span class="project-tag">Finance</span>
      </div>
    </div>
  </a>

  <a class="project-card" href="/posts/bounty-hunter-ai-local-bug-bounty-command-center/">
    <img src="/assets/img/projects/bounty-hunter-ai.png" alt="Bounty Hunter AI" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">Bounty Hunter AI</p>
      <p class="project-card-desc">Local ethical bug bounty command center. Passive recon orchestration, lead scoring, evidence viewer, payout tracker. Scope-enforced. No data leaves your machine.</p>
      <div class="project-tags">
        <span class="project-tag">Python</span>
        <span class="project-tag">FastAPI</span>
        <span class="project-tag">React</span>
        <span class="project-tag">Cybersecurity</span>
      </div>
    </div>
  </a>

  <a class="project-card" href="/posts/apex-paper-trading-terminal-tradingview-style-workspace-in-react/">
    <img src="/assets/img/projects/apex-trading-terminal.png" alt="Apex Trading Terminal" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">Apex Paper Trading Terminal</p>
      <p class="project-card-desc">TradingView-style paper trading workspace with live charts, watchlist, scanner, trade journal, and analytics. Backed by Alpaca paper trading.</p>
      <div class="project-tags">
        <span class="project-tag">React</span>
        <span class="project-tag">Alpaca</span>
        <span class="project-tag">Charts</span>
        <span class="project-tag">Trading</span>
      </div>
    </div>
  </a>

  <a class="project-card" href="/posts/trading-coach-saas-ai-powered-paper-trading-coach-concept/">
    <img src="/assets/img/projects/trading-coach-saas.png" alt="Trading Coach SaaS" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">Trading Coach SaaS</p>
      <p class="project-card-desc">Beginner-friendly AI paper-trading coach — guided setups, contextual feedback, progress tracking. SaaS product concept built with React and Claude API.</p>
      <div class="project-tags">
        <span class="project-tag">React</span>
        <span class="project-tag">SaaS</span>
        <span class="project-tag">AI</span>
        <span class="project-tag">Trading</span>
      </div>
    </div>
  </a>

  <a class="project-card" href="/posts/home-pro-business-website-for-a-family-remodeling-company/">
    <img src="/assets/img/projects/home-pro.png" alt="Home Pro" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">Home Pro</p>
      <p class="project-card-desc">Production-ready business website for a family-owned remodeling company serving Mississippi and Alabama. Lead gen, portfolio gallery, quote request flow.</p>
      <div class="project-tags">
        <span class="project-tag">React</span>
        <span class="project-tag">Tailwind</span>
        <span class="project-tag">Client Work</span>
      </div>
    </div>
  </a>

  <a class="project-card" href="/posts/pool-liners-premium-website-for-a-family-pool-business/">
    <img src="/assets/img/projects/pool-liners.png" alt="Pool Liners" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">Pool Liners Tennessee</p>
      <p class="project-card-desc">Premium lead-gen website for a family-owned Tennessee pool liner company. Mobile-first design, before/after gallery, free estimate request flow.</p>
      <div class="project-tags">
        <span class="project-tag">React</span>
        <span class="project-tag">Tailwind</span>
        <span class="project-tag">Client Work</span>
      </div>
    </div>
  </a>

  <a class="project-card" href="/posts/daytrader-bot-choch-fvg-automated-trading-strategy/">
    <img src="https://images.unsplash.com/photo-1611974789855-9c2a0a7236a3?w=600&q=80" alt="DayTrader Bot" loading="lazy">
    <div class="project-card-body">
      <p class="project-card-title">DayTrader Bot</p>
      <p class="project-card-desc">Automated day trading bot implementing the Craig Percoco CHoCH + Fair Value Gap strategy. Connects to Alpaca Paper Trading by default.</p>
      <div class="project-tags">
        <span class="project-tag">Python</span>
        <span class="project-tag">Alpaca</span>
        <span class="project-tag">Algo Trading</span>
        <span class="project-tag">CHoCH+FVG</span>
      </div>
    </div>
  </a>

</div>
