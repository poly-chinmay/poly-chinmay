# Hey, I'm Chinmay Aswale &nbsp;[![Website](https://img.shields.io/badge/chinmayaswale.com-000000?style=flat&logo=safari&logoColor=white)](https://chinmayaswale.com) [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/chinmay-aswale333)

> *I build AI systems that treat their own outputs as untrusted.*

3rd year Computer Engineering student @ SPPU, Pune. I work at the intersection of **agentic AI architecture**, **systems engineering**, and **quantitative finance**. My engineering philosophy: constrain non-determinism, validate at every boundary, rollback on failure.

&nbsp;

## ⚡ Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)

&nbsp;

## 🔒 Pinned Projects

### [Ghost.ai — Hardened Agentic Video Editor](https://github.com/poly-chinmay/ghost-ai)
> Rust · Python · LLM Pipeline · Multi-component Agent Architecture · React / Tauri

7-stage deterministic validation pipeline: `Parse → Schema Validation → Semantic Analysis → Safety Check → Preflight Simulation → Engine Execution → Commit`

LLM outputs treated as **untrusted objects** until validated across all seven stages. AppOrchestrator coordinates 9 independent engines — zero direct engine-to-engine calls.

| Metric | Result |
|--------|--------|
| Unsafe state transitions | **0** across 13 production phases |
| Orchestrated engines | **9** with no cross-dependencies |
| On failure | **Atomic rollback** — commits clean or reverts entirely |

---

### [Ultra-Low Latency Order Book Engine](https://github.com/poly-chinmay/order-book-engine)
> C++ · Lock-free Data Structures · Memory Pool Allocators

Limit order book matching engine targeting microsecond-range latency. Lock-free data structures, custom memory pool allocators, deterministic replay, and latency histogram visualisation benchmarked against naive STL implementation.

---

### [LLaMA-2-7B Supply Chain Fine-tune — AWS Deployed](https://github.com/poly-chinmay/llama-supply-chain)
> Python · LoRA · LLaMA-2 · AWS Lambda · API Gateway

Fine-tuned LLaMA-2-7B on 8,200 domain-specific supply chain Q&A pairs (LoRA r=8). Quantized and deployed as production REST API via AWS Lambda + API Gateway.

| Metric | Before | After |
|--------|--------|-------|
| Task-specific accuracy | 61% | **84%** |
| Inference latency | baseline | **↓22%** after quantization |

---

### [Mistral-7B — Indian Legal Judgment Summarization](https://github.com/poly-chinmay/mistral-legal)
> Python · LoRA · Mistral-7B-Instruct · A100

Fine-tuned Mistral-7B-Instruct on 14,500 cleaned Indian High Court & Supreme Court judgments for case summarization and precedent extraction. LoRA (r=16, α=32) — only ~0.8% of parameters trained.

| Metric | Before | After |
|--------|--------|-------|
| ROUGE-L | 0.41 | **0.63** |
| Hallucination rate | baseline | **↓28%** |
| Human factual accuracy | 62% | **85%** |

---

### [Reinforcement Learning Market Maker](https://github.com/poly-chinmay/rl-market-maker)
> Python · DQN · Custom Limit Order Book Simulator

DQN agent learning optimal bid-ask spread strategies. 2.5M timesteps trained against 3 years of historical crypto tick data.

| Metric | Before | After |
|--------|--------|-------|
| Sharpe Ratio | 0.8 | **1.9** |
| Max Drawdown | baseline | **↓17%** |
| Inventory Risk Variance | baseline | **↓31%** |

---

### [AI Inference Engine — Pure C++](https://github.com/poly-chinmay/ai-inference-cpp)
> C++ · SIMD · Manual Tensor Operations

Transformer forward pass implemented from scratch — no PyTorch, no external tensor libraries. Manual tensor operations with SIMD vectorisation for matrix multiplication. Benchmarked against PyTorch CPU baseline.

---

&nbsp;

## 📊 By the Numbers

| | |
|---|---|
| **20+** projects built | **3** LLMs fine-tuned |
| **1.9** best Sharpe ratio | **3+** production sites deployed |
| **14,500** legal judgments processed | **0** unsafe AI state transitions |

&nbsp;

## 🎯 Currently

- 🔨 Building **Ghost.ai** — hardened agentic pipeline in Rust
- 📖 Preparing for **CFA Level 1** — August 2026
- 🌐 Running **DPMUN 2026** — [dpmun.in](https://dpmun.in)
- 🎯 Open to **AI infrastructure & quant internships — 2026**

&nbsp;

## 📬 Reach Me

[![Email](https://img.shields.io/badge/poly.chinmay@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:poly.chinmay@gmail.com)
[![Website](https://img.shields.io/badge/chinmayaswale.com-000000?style=flat&logo=safari&logoColor=white)](https://chinmayaswale.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/chinmay-aswale333)

---

<sub><i>"The LLM never touches application state directly." — Ghost.ai architecture doc</i></sub>
