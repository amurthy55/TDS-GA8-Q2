---
marp: true
theme: gaia
paginate: true
paginator: true
pageNumber: true
footer: "Contact: 25ds2000003@ds.study.iitm.ac.in | IIT Madras"
style: |
  section {
    font-family: "Helvetica Neue", Arial, sans-serif;
    color: #222;
  }
  section.lead h1 {
    color: #1a5fb4;
    text-align: center;
    font-size: 2.2em;
  }
  section::after {
    content: attr(data-marpit-pagination) " / " attr(data-marpit-pagination-total);
    color: #666;
    font-size: 0.8em;
  }
  code {
    background: #f4f4f4;
    padding: 2px 6px;
    border-radius: 4px;
  }
  pre {
    background: #2d2d2d !important;
    color: #f8f8f2 !important;
    border-radius: 8px;
  }
  blockquote {
    border-left: 5px solid #1a5fb4;
    background: #f0f4f8;
    padding: 1em;
    margin: 1em 0;
  }
---

<!-- _theme: gaia -->
<!-- _class: lead gaia -->
<!-- backgroundColor: #0d3b66 -->

![bg opacity:0.3](https://images.unsplash.com/photo-1518432031352-d65fc6c30292?ixlib=rb-4.0.3&auto=format&fit=crop&w=2000&q=80)

# Product Documentation  
**AcmeFlow v2.4**  
High-Performance Data Pipeline Engine

<span style="font-size:0.7em; color:#faf0ca">25ds2000003@ds.study.iitm.ac.in</span>

---

# Why AcmeFlow?

- **Blazing fast** processing with zero-copy architecture
- **Fault-tolerant** streaming with exactly-once semantics
- Supports **real-time** and **batch** workloads
- Built on Rust for memory safety and performance

> "AcmeFlow reduced our pipeline latency from 12s to 180ms"  
> — Lead Engineer, Fortune 500 Bank

---

# Core Architecture

```mermaid
graph TD
    A[Source Connectors] --> B[Processing Engine]
    B --> C[Transformation Nodes]
    C --> D[Sink Connectors]
    B --> E[State Store (RocksDB)]
    E --> B
    style B fill:#1a5fb4,stroke:#fff,color:#fff
