---
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
  section {
    background: #f6f7fa;
    color: #222;
    font-family: 'Segoe UI', system-ui, sans-serif;
  }
  h1, h2, h3 { 
    color: #0d47a1; 
    font-weight: 700;
  }
  a { color: #007bff; }
  code { 
    background: #e3f2fd; 
    padding: 2px 6px; 
    border-radius: 4px; 
    font-size: 0.9em;
  }
  pre { background: #263238 !important; color: #cddc39 !important; }
  section::after {
    font-size: 0.75em;
    color: #666;
  }
---

<!-- _class: lead -->
![bg opacity:0.25](https://images.unsplash.com/photo-1517180107641-cdf0c8122361?auto=format&fit=crop&q=90&w=2400)

# Product Documentation Presentation

### 25ds2000003@ds.study.iitm.ac.in  
*IIT Madras – Diploma in Data Science*

---

# Documentation Goals

- Fully version-controlled with Git
- One source → HTML • PDF • PPTX
- Engineer-friendly Markdown syntax
- Full support for LaTeX math, code, diagrams, and backgrounds

> This deck is written entirely in Markdown + Marp

---

# Product Overview – AcmeSDK v3

- TypeScript-first SDK
- REST + GraphQL clients
- Built-in resilience (retry, circuit-breaker, rate limiting)
- 99.99% SLA

---

# Installation

```bash
npm install @acme/sdk
