---
marp: true
theme: default
paginate: true
size: 16:9
style: |
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
  
  section {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, sans-serif;
    background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
    color: #f8f9fa;
    padding: 60px;
  }
  
  section.lead {
    text-align: center;
    justify-content: center;
    background: linear-gradient(135deg, #0f3460 0%, #1a1a2e 100%);
  }
  
  section.lead h1 {
    font-size: 4rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    color: #00d4ff;
  }
  
  section.lead h3 {
    font-size: 1.8rem;
    font-weight: 400;
    opacity: 0.9;
    margin-top: 1rem;
    color: #a8d0f0;
  }
  
  h1, h2 {
    color: #00d4ff;
    font-weight: 600;
  }
  
  h3 {
    color: #ffd700;
    font-weight: 500;
  }
  
  section ul {
    font-size: 1.1rem;
    line-height: 1.6;
  }
  
  section li {
    margin-bottom: 0.8rem;
  }
  
  strong {
    color: #fff;
    font-weight: 600;
  }
  
  table {
    background: rgba(255, 255, 255, 0.95);
    border-radius: 8px;
    backdrop-filter: blur(10px);
    color: #1a1a2e;
    margin: 20px auto;
  }
  
  th, td {
    border: 1px solid rgba(26, 26, 46, 0.15);
    padding: 15px 20px;
    text-align: left;
  }
  
  th {
    background: rgba(0, 212, 255, 0.1);
    font-weight: 600;
    color: #0f3460;
  }
  
  blockquote {
    background: rgba(255, 215, 0, 0.15);
    border-left: 4px solid #ffd700;
    padding: 20px;
    border-radius: 8px;
    font-style: italic;
    font-size: 1.2rem;
    color: #f8f9fa;
  }
  
  .highlight-box {
    background: rgba(0, 212, 255, 0.1);
    border: 2px solid rgba(0, 212, 255, 0.3);
    border-radius: 12px;
    padding: 24px;
    margin: 20px 0;
    backdrop-filter: blur(10px);
  }
  
  .metrics {
    display: flex;
    justify-content: space-around;
    margin: 30px 0;
  }
  
  .metric {
    text-align: center;
    padding: 20px;
    background: rgba(255, 255, 255, 0.1);
    border-radius: 8px;
    backdrop-filter: blur(10px);
  }
  
  .metric-number {
    font-size: 2.5rem;
    font-weight: 700;
    color: #00d4ff;
    display: block;
  }
  
  .metric-label {
    font-size: 0.9rem;
    opacity: 0.8;
    margin-top: 5px;
  }
---

<!-- class: lead -->

# On-chain Portfolio Autopilot  
### Zap Pilot

---

### One-liner

> **With one click, Zap Pilot locks in profits, buys the dips, and shifts your crypto to higher-yield pools — all in under 30 seconds every six months, while you keep full control of your wallet.**

---

## The Problem

<div class="highlight-box">

**Active crypto holders juggle 5+ chains, 10+ dApps**

Current painful manual workflow:
1. Bridge assets across chains  
2. Swap into target tokens  
3. Claim & sell farming rewards  
4. Re-allocate to higher-APR pools  
5. Repeat for every wallet

</div>

- Manual rebalancing takes **30–45 min** and frequent gas fees  
- Vault protocols demand **custody & performance fees**  
- Result: portfolios drift, rewards pile up, alpha is lost

*⇨ 8–10 transactions, dozens of clicks, every rebalance cycle*

---

## Solution — Zap Pilot

**One-click “Rebalance” button** that:

- Sweeps dust & claims rewards  
- Sells winners, buys laggards  
- Routes funds to higher-yield pools  
- Respects user rules (e.g. “≥ 50 % stables”)  
- Signs everything **from the user’s own wallet**

_Time spent: < 30 s • Custody: 100 % user-held_

---

## How it works (under the hood)

| Step | Tech |
|------|------|
| Intent batching | ERC-4337 AA wallets |
| Cross-chain routing | LayerZero / Axelar bridges |
| Yield discovery | On-chain APR oracle |
| Policy engine | JSON rules → execution DAG |
| Security | Audited, non-upgradeable modules |

---

## Demo

<div class="highlight-box">

### 🎯 **One-Click Rebalance Demo**

**Before**: 45 minutes, 8-10 transactions, multiple dApps
**After**: 30 seconds, 1 signature, Zap Pilot handles everything

*Replace with actual demo video/GIF when available*

</div>

---

## Why we win

- **Self-custodial** — no vault lock-in, no counter-party risk  
- **Time alpha** — 30 s vs 45 min per cycle  
- **Rule-based control** — user chooses weights, frequency, risk caps  
- **Composability** — plug-in to any wallet or DAO multisig

---

## Market & Business Model

<div class="metrics">
<div class="metric">
<span class="metric-number">25M</span>
<span class="metric-label">Self-custodial DeFi wallets</span>
</div>
<div class="metric">
<span class="metric-number">$90B</span>
<span class="metric-label">Addressable crypto AUM</span>
</div>
<div class="metric">
<span class="metric-number">$900M</span>
<span class="metric-label">Target AUM (1% penetration)</span>
</div>
</div>

### Revenue Model

| Plan | Offering | Revenue |
|------|----------|---------|
| **Free** | Manual one-click rebalance | 0.2% optional tip |
| **Pro** | Scheduled rebalances, advanced rules | $12/mo |
| **Enterprise** | DAO treasury dashboard & APIs | Custom pricing |

---

## Traction & Roadmap

<div class="highlight-box">

### Current Traction (8 weeks closed beta)

<div class="metrics">
<div class="metric">
<span class="metric-number">$3.5M</span>
<span class="metric-label">TVL managed</span>
</div>
<div class="metric">
<span class="metric-number">19.8%</span>
<span class="metric-label">Avg net APY delivered</span>
</div>
<div class="metric">
<span class="metric-number">720+</span>
<span class="metric-label">Successful rebalances</span>
</div>
<div class="metric">
<span class="metric-number">0</span>
<span class="metric-label">Custody incidents</span>
</div>
</div>

**Integrations**: MetaMask Snaps, Rabby, Safe{Wallet}

</div>

### Roadmap

| Q3 '25 | Q4 '25 | Q1 '26 |
|--------|--------|--------|
| Launch public beta<br>Pro subscription | DAO/multisig module<br>Mobile SDK | AI yield-signal engine<br>Reflexive fee sharing |

---

## Team & Ask

<div class="highlight-box">

### 👥 **Core Team**

| Role | Background |
|------|------------|
| **David H.** | ex-MakerDAO engineer, 6 yrs DeFi |
| **Alice C.** | Ex-Bloomberg quant, risk models |
| **Ken L.** | Google SRE → infra & security |
| **Advisors** | Steven (Press Start Capital), Jane (ex-IndexCoop) |

</div>

---

<!-- _class: lead -->

# 🚀 **The Ask**

**Raising $2.5M seed round**  
18-month runway • 10% equity  

<br>

### 📧 Contact
**david@zap-pilot.org** | **@zap-pilot**

<br>

## Thank you! 🙏
