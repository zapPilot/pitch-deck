---
marp: true
theme: gaia
paginate: true
size: 16:9
backgroundColor: #1a1a2e
color: #f8f9fa
style: |
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600&display=swap');
  
  :root {
    --primary-color: #00d4ff;
    --secondary-color: #ffd700;
    --accent-color: #ff6b6b;
    --dark-bg: #1a1a2e;
    --darker-bg: #16213e;
    --light-text: #f8f9fa;
    --muted-text: #a8d0f0;
  }
  
  section {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, sans-serif;
    background: linear-gradient(135deg, var(--dark-bg) 0%, var(--darker-bg) 100%);
    color: var(--light-text);
    padding: 60px;
    position: relative;
    overflow: hidden;
  }
  
  section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 20% 80%, rgba(0, 212, 255, 0.03) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 215, 0, 0.03) 0%, transparent 50%);
    pointer-events: none;
    z-index: -1;
  }
  
  section.lead {
    text-align: center;
    justify-content: center;
    background: linear-gradient(135deg, #0f3460 0%, var(--dark-bg) 100%);
    position: relative;
  }
  
  section.lead::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      radial-gradient(circle at 50% 50%, rgba(0, 212, 255, 0.1) 0%, transparent 70%),
      linear-gradient(45deg, transparent 30%, rgba(255, 215, 0, 0.05) 50%, transparent 70%);
    pointer-events: none;
    z-index: -1;
  }
  
  section.lead h1 {
    font-size: 4.5rem;
    font-weight: 900;
    margin-bottom: 0.5rem;
    color: var(--primary-color);
    text-shadow: 0 0 30px rgba(0, 212, 255, 0.3);
    line-height: 1.1;
  }
  
  section.lead h3 {
    font-size: 2rem;
    font-weight: 500;
    opacity: 0.9;
    margin-top: 1rem;
    color: var(--muted-text);
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
  }
  
  h1, h2 {
    color: var(--primary-color);
    font-weight: 700;
    text-shadow: 0 2px 10px rgba(0, 212, 255, 0.2);
    margin-bottom: 1.5rem;
    position: relative;
  }
  
  h1::after, h2::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 0;
    width: 60px;
    height: 3px;
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
    border-radius: 2px;
  }
  
  h3 {
    color: var(--secondary-color);
    font-weight: 600;
    text-shadow: 0 1px 5px rgba(255, 215, 0, 0.2);
  }
  
  section ul {
    font-size: 1.1rem;
    line-height: 1.6;
    text-align: left;
    padding-left: 1.5rem;
  }
  
  section li {
    margin-bottom: 0.8rem;
    text-align: left;
  }
  
  strong {
    color: #fff;
    font-weight: 600;
  }
  
  table {
    background: rgba(255, 255, 255, 0.95);
    border-radius: 12px;
    backdrop-filter: blur(15px);
    color: var(--dark-bg);
    margin: 30px auto;
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
    border: 1px solid rgba(255, 255, 255, 0.2);
    overflow: hidden;
  }
  
  th, td {
    border: none;
    border-bottom: 1px solid rgba(26, 26, 46, 0.1);
    padding: 18px 24px;
    text-align: left;
  }
  
  th {
    background: linear-gradient(135deg, rgba(0, 212, 255, 0.1) 0%, rgba(255, 215, 0, 0.05) 100%);
    font-weight: 700;
    color: var(--darker-bg);
    text-transform: uppercase;
    font-size: 0.9rem;
    letter-spacing: 0.5px;
  }
  
  tr:last-child td {
    border-bottom: none;
  }
  
  td {
    font-weight: 500;
  }
  
  blockquote {
    background: linear-gradient(135deg, rgba(255, 215, 0, 0.1) 0%, rgba(0, 212, 255, 0.05) 100%);
    border-left: 4px solid var(--secondary-color);
    padding: 30px;
    border-radius: 12px;
    font-style: italic;
    font-size: 1.4rem;
    color: var(--light-text);
    margin: 30px 0;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
    position: relative;
    font-weight: 500;
  }
  
  blockquote::before {
    content: '"';
    position: absolute;
    top: -10px;
    left: 20px;
    font-size: 4rem;
    color: var(--secondary-color);
    opacity: 0.3;
    font-family: serif;
  }
  
  .highlight-box {
    background: linear-gradient(135deg, rgba(0, 212, 255, 0.08) 0%, rgba(255, 215, 0, 0.05) 100%);
    border: 2px solid rgba(0, 212, 255, 0.3);
    border-radius: 16px;
    padding: 32px;
    margin: 30px 0;
    backdrop-filter: blur(15px);
    box-shadow: 
      0 8px 32px rgba(0, 0, 0, 0.3),
      inset 0 1px 0 rgba(255, 255, 255, 0.1);
    position: relative;
    overflow: hidden;
  }
  
  .highlight-box::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 2px;
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
    z-index: 1;
  }
  
  .metrics {
    display: flex;
    justify-content: space-around;
    margin: 40px 0;
    gap: 20px;
  }
  
  .metric {
    text-align: center;
    padding: 30px 25px;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.08) 0%, rgba(0, 212, 255, 0.05) 100%);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 16px;
    backdrop-filter: blur(20px);
    box-shadow: 
      0 8px 32px rgba(0, 0, 0, 0.2),
      inset 0 1px 0 rgba(255, 255, 255, 0.1);
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
  }
  
  .metric::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 2px;
    background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
    transform: scaleX(0);
    transition: transform 0.3s ease;
  }
  
  .metric:hover::before {
    transform: scaleX(1);
  }
  
  .metric:hover {
    transform: translateY(-5px);
    box-shadow: 
      0 12px 40px rgba(0, 0, 0, 0.3),
      inset 0 1px 0 rgba(255, 255, 255, 0.2);
  }
  
  .metric-number {
    font-size: 3rem;
    font-weight: 900;
    color: var(--primary-color);
    display: block;
    text-shadow: 0 0 20px rgba(0, 212, 255, 0.3);
    font-family: 'JetBrains Mono', monospace;
  }
  
  .metric-label {
    font-size: 1rem;
    opacity: 0.8;
    margin-top: 8px;
    color: var(--muted-text);
    font-weight: 500;
  }
---

<!-- class: lead -->

# Zap Pilot
### On-chain Portfolio Autopilot  

---

### One-liner

> **With one click, Zap Pilot locks in profits, buys the dips, and shifts your crypto to higher-yield pools — all in under 30 seconds every six months, while you keep full control of your wallet.**

---

## The Problem

### Active crypto holders juggle 5+ chains, 10+ dApps

**Current painful manual workflow:**

1. **Bridge assets** across chains  
2. **Swap** into target tokens  
3. **Claim & sell** farming rewards  
4. **Re-allocate** to higher-APR pools  

<div class="highlight-box">

**The Pain Points:**

• Manual rebalancing takes **30–45 minutes** + frequent gas fees  
• Vault protocols demand **custody & performance fees**  
• Result: 30–45 min lost per rebalance, allocations drift

**⇨ 8–10 transactions, dozens of clicks, every rebalance cycle**

</div>

---

## Solution — Zap Pilot

<div class="highlight-box">

### 🎯 **One-click "Optimize"**

**What it does:**

• **Sweeps dust** & claims rewards  
• **Sells winners**, buys laggards  
• **Routes funds** to higher-yield pools  
• **100 % self-custody** — you sign every step; funds never leave your wallet


</div>

<div class="metrics">
<div class="metric">
<span class="metric-number">< 30s</span>
<span class="metric-label">Time spent</span>
</div>
<div class="metric">
<span class="metric-number">100%</span>
<span class="metric-label">User-held custody</span>
</div>
<div class="metric">
<span class="metric-number">1</span>
<span class="metric-label">Click to rebalance</span>
</div>
</div>

---

## How it works (under the hood)

| Step | Tech |
|------|------|
| Intent batching | EIP-7702 EOA wallets |
| Cross-chain routing | Across / Squid bridges |
| Security | 0 smart contract, 100% in your wallet |

---

## Demo

<div class="highlight-box">

### 🎯 **One-Click Rebalance Demo**

**Before**: 30 minutes, 8-10 transactions, multiple dApps
**After**: 30 seconds, 1 signature, Zap Pilot handles everything

*Replace with actual demo video/GIF when available*

</div>

---

## Why we win

- **Self-custodial** — no vault lock-in, no counter-party risk  
- **Time alpha** — 30 s vs 30 min per cycle  

---

## Market & Business Model

<div class="metrics">
<div class="metric">
<span class="metric-number">220K</span>
<span class="metric-label">Self-custodial DeFi wallets</span>
</div>
<div class="metric">
<span class="metric-number">$XXB</span>
<span class="metric-label">Addressable crypto AUM</span>
</div>
<div class="metric">
<span class="metric-number">$XXM</span>
<span class="metric-label">Target AUM (1% penetration)</span>
</div>
</div>

---

### Revenue Model

| Plan | Offering | Revenue |
|------|----------|---------|
| **Free** | Manual one-click zap in/out and rebalance | 1% entry fee |

---

## Team & Ask

<div class="highlight-box">

### 👥 **Core Team**

| Role | Background |
|------|------------|
| **David Chang** | Ex-Dcard Engineer, 3 yrs DeFi |
| **Adrian Wu** | Microsoft PM, Business Development Advisor
| **Eric Chan** | Ex-Dcard Engineer, Strategy Advisor |

</div>

---

### 📧 Contact

![X/Twitter](./qrcode.png)

**zappilot.eth@ud.me / davidtnfsh@gmail.com** 

<br>

## Thank you! 🙏
