<div align="center">

<!-- ANIMATED WAVE HEADER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=220&section=header&text=Chinmay%20Aswale&fontSize=62&fontColor=ffffff&fontAlignY=38&desc=I%20build%20AI%20systems%20that%20treat%20their%20own%20outputs%20as%20untrusted.&descSize=17&descAlignY=58&descColor=a78bfa&animation=fadeIn" width="100%"/>

<!-- ANIMATED TYPING -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=800&color=4F6EF7&center=true&vCenter=true&multiline=false&repeat=true&width=750&height=50&lines=Agentic+AI+Architect+%F0%9F%94%92;Systems+Engineer+%E2%9A%A1;Quant+%2F+RL+Researcher+%F0%9F%93%88;LLM+Fine-tuner+%F0%9F%A7%A0;NeurIPS+2026+Researcher+%F0%9F%93%9D;Full-stack+Builder+%F0%9F%8C%90" alt="Typing SVG" />

<br/><br/>

[![Open to Internships](https://img.shields.io/badge/🎯_Open_to-AI_Infra_%26_Quant_Internships_2026-4f6ef7?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)
[![Research](https://img.shields.io/badge/📝_Research-NeurIPS_2026_Workshop_(Pre--submission)-a78bfa?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)
[![CFA](https://img.shields.io/badge/📖_CFA-Level_1_Aug_2026-f59e0b?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)
[![Location](https://img.shields.io/badge/📍-Pune,_India-10b981?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)

</div>

---

## 🧠 About

```python
chinmay = {
    "role"      : "3rd Year Computer Engineering @ SPPU, Pune",
    "focus"     : ["Agentic AI Architecture", "Systems Engineering", "Quant Finance"],
    "research"  : "Deterministic Neural Execution for Periodic Scheduling Policy Evaluation",
    "target"    : "NeurIPS 2026 Workshop (Pre-submission)",
    "building"  : "Ghost.ai — hardened agentic pipeline in Rust",
    "philosophy": "constrain non-determinism · validate at every boundary · rollback on failure",
    "currently" : "Open to AI Infrastructure & Quant internships — 2026"
}
```

---

## ⚡ Stack

<div align="center">

**Languages**

[![Rust](https://img.shields.io/badge/Rust-ef8a4e?style=for-the-badge&logo=rust&logoColor=white)]()
[![C++](https://img.shields.io/badge/C++-4f6ef7?style=for-the-badge&logo=cplusplus&logoColor=white)]()
[![Python](https://img.shields.io/badge/Python-facc15?style=for-the-badge&logo=python&logoColor=black)]()
[![SQL](https://img.shields.io/badge/SQL-475569?style=for-the-badge&logo=postgresql&logoColor=white)]()

**AI / Agentic**

[![LLM Pipelines](https://img.shields.io/badge/LLM_Pipelines-a78bfa?style=for-the-badge)]()
[![LoRA Fine-tuning](https://img.shields.io/badge/LoRA_%2F_QLoRA-7c3aed?style=for-the-badge)]()
[![Multi-Agent Orchestration](https://img.shields.io/badge/Multi--Agent_Orchestration-4f6ef7?style=for-the-badge)]()
[![RAG](https://img.shields.io/badge/RAG_Pipelines-6366f1?style=for-the-badge)]()

**ML / Quant**

[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white)]()
[![RL](https://img.shields.io/badge/Reinforcement_Learning-10b981?style=for-the-badge)]()
[![Monte Carlo](https://img.shields.io/badge/Monte_Carlo_Simulation-059669?style=for-the-badge)]()

**Systems**

[![Lock-free](https://img.shields.io/badge/Lock--free_Data_Structures-ef4444?style=for-the-badge)]()
[![SIMD](https://img.shields.io/badge/SIMD_%2F_AVX2-dc2626?style=for-the-badge)]()
[![eBPF](https://img.shields.io/badge/eBPF-f97316?style=for-the-badge)]()
[![Event Sourcing](https://img.shields.io/badge/Event_Sourcing-b45309?style=for-the-badge)]()

**Cloud**

[![AWS](https://img.shields.io/badge/AWS_Lambda_%2B_API_Gateway-232F3E?style=for-the-badge&logo=amazonaws&logoColor=FF9900)]()
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)]()
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)]()

</div>

---

## 📝 Research

### Deterministic Neural Execution for Periodic Scheduling Policy Evaluation
> *Formally Bounded Latency and Statistical Generalization Guarantees*
> **Target: NeurIPS 2026 Workshop** · Pre-submission · Submitted for Faculty Review

| Contribution | Detail |
|-------------|--------|
| ⏱️ Formal latency bound | **152 μs worst-case** — derived analytically from architecture params |
| 🔒 Collapse operator | Deterministic, unique, order-independent — proven via integer arithmetic |
| 📐 Representational sufficiency | F₂ policy class — architectural guarantee, not training assumption |
| 📊 Generalization bound | Bartlett & Shawe-Taylor — all 9 assumptions stated explicitly |

---

## 🔒 Featured Projects

### 👻 [Ghost.ai — Hardened Agentic Video Editor](https://github.com/poly-chinmay/ghost-ai)
> `Rust` `Python` `LLM Pipeline` `Tauri` `React` `Event Sourcing`

**The LLM never touches application state directly.**

```
User → [LLM] → UntrustedAIResponse
                      ↓
    ┌─────── 7-Stage Validation Pipeline ───────┐
    │  Parse → Schema → Semantic → Safety       │
    │  → Preflight → Execute → Commit           │
    └───────────────────┬───────────────────────┘
                        ↓
          ✅ Clean Commit  |  🔄 Atomic Rollback
```

| Metric | Value |
|--------|-------|
| 🟢 Unsafe state transitions | **0** across 13 production phases |
| ⚙️ Engines orchestrated | **9** independent — zero cross-talk |
| 🔄 Failure mode | Atomic rollback — clean commit or full revert |

---

### ⚡ [Ultra-Low Latency Order Book Engine](https://github.com/poly-chinmay/order-book-engine)
> `C++` `Lock-free DS` `Memory Pool Allocators` `SIMD`

Microsecond-range limit order book matching. Lock-free structures, custom memory pools, deterministic replay. Benchmarked vs naive STL.

---

### 🧠 [LLaMA-2-7B — Supply Chain Fine-tune (AWS Deployed)](https://github.com/poly-chinmay/llama2-supply-chain)
> `Python` `LoRA r=8` `AWS Lambda` `API Gateway` `Quantization`

| Metric | Before | After |
|--------|--------|-------|
| Task accuracy | 61% | **84%** |
| Inference latency | baseline | **↓22%** post-quantization |
| Deployment | — | **Production REST API on AWS** |

---

### ⚖️ [Mistral-7B — Indian Legal Judgment Summarization](https://github.com/poly-chinmay/mistral-7b-legal-india)
> `Python` `LoRA r=16, α=32` `Mistral-7B-Instruct` `A100 40GB`

14,500 High Court & Supreme Court judgments · ~0.8% trainable params

| ROUGE-L | Hallucination Rate | Human Factual Accuracy |
|---------|-------------------|----------------------|
| 0.41 → **0.63** | **↓28%** | 62% → **85%** |

---

### 📈 [Reinforcement Learning Market Maker](https://github.com/poly-chinmay/rl-market-maker)
> `Python` `DQN` `Reward Shaping` `Custom LOB Simulator`

2.5M timesteps · 3 years historical crypto tick data

| Sharpe Ratio | Max Drawdown | Inventory Risk Variance |
|-------------|-------------|------------------------|
| 0.8 → **1.9** | **↓17%** | **↓31%** |

---

### ⚙️ [AI Inference Engine — Pure C++](https://github.com/poly-chinmay/ai-inference-cpp)
> `C++` `SIMD AVX2` `Manual Tensor Ops` — Zero external dependencies

Transformer forward pass from scratch. No PyTorch. SIMD-optimised matmul benchmarked vs PyTorch CPU.

---

### 🏥 [Falcon-7B — Medical QA Fine-tune](https://github.com/poly-chinmay/falcon-7b-medical-qa)
> `Python` `LoRA r=32` `Falcon-7B` `A100`

| BLEU Score | Critical Factual Error Rate |
|-----------|---------------------------|
| **↑18%** | **↓37%** |

---

## 📊 By the Numbers

<div align="center">

[![](https://img.shields.io/badge/Projects_Built-20+-4f6ef7?style=for-the-badge&labelColor=0a0a0f)]()
[![](https://img.shields.io/badge/LLMs_Fine--tuned-4-7c3aed?style=for-the-badge&labelColor=0a0a0f)]()
[![](https://img.shields.io/badge/Best_Sharpe_Ratio-1.9-10b981?style=for-the-badge&labelColor=0a0a0f)]()
[![](https://img.shields.io/badge/Production_Sites-3+-f59e0b?style=for-the-badge&labelColor=0a0a0f)]()
[![](https://img.shields.io/badge/Legal_Judgments_Processed-14.5k-ef4444?style=for-the-badge&labelColor=0a0a0f)]()
[![](https://img.shields.io/badge/Unsafe_AI_State_Transitions-0-22c55e?style=for-the-badge&labelColor=0a0a0f)]()
[![](https://img.shields.io/badge/Worst--case_Inference_Latency-152μs-f97316?style=for-the-badge&labelColor=0a0a0f)]()

</div>

---

## 📈 GitHub Stats

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=poly-chinmay&theme=midnight_purple" width="100%"/>

</div>

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=poly-chinmay&theme=midnight_purple" height="160em"/>
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=poly-chinmay&theme=midnight_purple" height="160em"/>
<img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=poly-chinmay&theme=midnight_purple" height="160em"/>
<img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=poly-chinmay&theme=midnight_purple&utcOffset=5.5" height="160em"/>

</div>

<div align="center">

<img src="https://streak-stats.demolab.com/?user=poly-chinmay&theme=midnight-purple&hide_border=true&background=0a0a0f&stroke=4f6ef7&ring=a78bfa&fire=f59e0b&currStreakLabel=4f6ef7" width="100%"/>

</div>

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=poly-chinmay&bg_color=0a0a0f&color=4f6ef7&line=a78bfa&point=f59e0b&area=true&hide_border=true" width="100%"/>

</div>

<!-- Auto-generated by GitHub Actions daily — populated once code is pushed -->
<div align="center">
<img src="github-metrics.svg" alt="Metrics" width="100%"/>
</div>

---

## 🌐 Production

| Project | Stack | Live |
|---------|-------|------|
| DPMUN 2026 Conference Platform | Next.js · Custom Backend · Payment Gateway | [dpmun.in](https://dpmun.in) |
| Personal Site | — | [chinmayaswale.com](https://chinmayaswale.com) |

---

## 📬 Connect

<div align="center">

[![Website](https://img.shields.io/badge/chinmayaswale.com-4f6ef7?style=for-the-badge&logo=safari&logoColor=white)](https://chinmayaswale.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/chinmay-aswale333)
[![Email](https://img.shields.io/badge/poly.chinmay@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:poly.chinmay@gmail.com)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer&animation=fadeIn" width="100%"/>

*"The LLM never touches application state directly." — Ghost.ai architecture doc*

</div>
