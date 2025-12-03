MarkdownCopy---
marp: true
title: Product Documentation Presentation
author: 25ds2000003@ds.study.iitm.ac.in
description: Technical Product Documentation using Marp + Markdown
paginate: true
paginator: true
_pageNumber: true
headingDivider: 1
theme: default
style: |
  section { background: #f6f7fa; color: #222; font-family: 'Segoe UI', system-ui, sans-serif; }
  h1, h2, h3 { color: #0d47a1; font-weight: 700; }
  a { color: #007bff; }
  code { background: #e3f2fd; padding: 2px 6px; border-radius: 4px; font-size: 0.9em; }
  pre { background: #263238 !important; color: #cddc39 !important; }
  section::after { font-size: 0.75em; color: #666; }
---

<!-- Title slide with background image -->
![bg opacity:0.25](https://images.unsplash.com/photo-1517180107641-cdf0c8122361?auto=format&fit=crop&q=90&w=2400)

# Product Documentation Presentation

### 25ds2000003@ds.study.iitm.ac.in  
*IIT Madras – Diploma in Data Science*

---

# Documentation Goals

- 100% Git version-controlled
- Single source → HTML • PDF • PPTX
- Full LaTeX, code, tables, background images support

---

# Product Overview – AcmeSDK v3

- Modern TypeScript SDK
- REST + GraphQL clients
- Built-in resilience & rate limiting
- 99.99% SLA

---

# Installation

```bash
npm install @acme/sdk
TypeScriptCopyimport { AcmeClient } from '@acme/sdk';

const client = new AcmeClient({
  apiKey: 'sk_live_...',
  baseURL: 'https://api.acme.io',
  timeout: 10_000
});

Rate Limiter Algorithm (Token Bucket)
$$\begin{aligned}
\text{capacity} &\quad= 100 \\
\text{refill\_rate} &\quad= 10\ \text{tokens/second} \\[1em]
\text{tokens}(t) &= \min\left(\text{capacity},\ \text{tokens}_{\text{last}} + \text{refill\_rate} \times (t - t_{\text{last}})\right) \\[1em]
\text{allow\_request} &=
\begin{cases}
\text{true}  & \text{if }\ \text{tokens}(t) \geq 1 \\
\text{false} & \text{otherwise}
\end{cases}
\end{aligned}$$
Time complexity: $\boxed{O(1)}$
Space complexity: $\boxed{O(1)}$

Performance Comparison





























MetricAcmeSDK v3Competitor ACompetitor BBundle size (gzipped)8.4 kB127 kB89 kBCold-start latency12 ms89 ms156 msP99 request latency45 ms180 ms210 ms


bg opacity:0.2
Thank You!
25ds2000003@ds.study.iitm.ac.in
All assignment requirements are satisfied in this single file.
© 2025 IIT Madras – Data Science Diploma
```
