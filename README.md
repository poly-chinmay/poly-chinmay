<div align="center">

<!-- ANIMATED WAVE HEADER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=Chinmay%20Aswale&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=I%20build%20AI%20systems%20that%20treat%20their%20own%20outputs%20as%20untrusted.&descSize=16&descAlignY=58&descColor=a78bfa&animation=fadeIn" width="100%"/>

<!-- ANIMATED TYPING -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1000&color=4F6EF7&center=true&vCenter=true&multiline=false&repeat=true&width=700&height=50&lines=Agentic+AI+Architect+%F0%9F%94%92;Systems+Engineer+%E2%9A%A1;Quant+%2F+RL+Researcher+%F0%9F%93%88;LLM+Fine-tuner+%F0%9F%A7%A0;Full-stack+Builder+%F0%9F%8C%90" alt="Typing SVG" />

<br/>

[![Open to Internships](https://img.shields.io/badge/🎯_Open_to-AI_Infra_%26_Quant_Internships_2026-4f6ef7?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)
[![CFA Level 1](https://img.shields.io/badge/📖_CFA-Level_1_Aug_2026-f59e0b?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)
[![SPPU](https://img.shields.io/badge/🎓_SPPU-3rd_Year_CE-10b981?style=for-the-badge&labelColor=0a0a0f)](https://chinmayaswale.com)

<br/><br/>

</div>

---

## ⚡ Stack

<div align="center">

**Languages**

![Rust](https://img.shields.io/badge/Rust-ef8a4e?style=for-the-badge&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/C++-4f6ef7?style=for-the-badge&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-facc15?style=for-the-badge&logo=python&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-64748b?style=for-the-badge&logo=postgresql&logoColor=white)

**AI / Agentic Systems**

![LLM Pipelines](https://img.shields.io/badge/LLM_Pipelines-a78bfa?style=for-the-badge&logoColor=white)
![LoRA Fine-tuning](https://img.shields.io/badge/LoRA_Fine--tuning-7c3aed?style=for-the-badge&logoColor=white)
![Multi-Agent Orchestration](https://img.shields.io/badge/Multi--Agent_Orchestration-4f6ef7?style=for-the-badge&logoColor=white)
![RAG](https://img.shields.io/badge/RAG_Pipelines-6366f1?style=for-the-badge&logoColor=white)

**ML / Quant**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white)
![Reinforcement Learning](https://img.shields.io/badge/Reinforcement_Learning-10b981?style=for-the-badge&logoColor=white)
![Monte Carlo](https://img.shields.io/badge/Monte_Carlo_Sim-059669?style=for-the-badge&logoColor=white)

**Systems**

![Lock-free DS](https://img.shields.io/badge/Lock--free_Data_Structures-ef4444?style=for-the-badge&logoColor=white)
![SIMD](https://img.shields.io/badge/SIMD_/_AVX2-dc2626?style=for-the-badge&logoColor=white)
![eBPF](https://img.shields.io/badge/eBPF-f97316?style=for-the-badge&logoColor=white)
![Event Sourcing](https://img.shields.io/badge/Event_Sourcing-b45309?style=for-the-badge&logoColor=white)

**Cloud & Deploy**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=FF9900)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)

</div>

---

## 🔒 Featured Projects

### 👻 [Ghost.ai — Hardened Agentic Video Editor](https://github.com/poly-chinmay/ghost-ai)

> `Rust` `Python` `LLM Pipeline` `Tauri` `React` `Event Sourcing`

**Core principle:** The LLM never touches application state directly.

```
User → [LLM] → UntrustedAIResponse
                      ↓
    ┌─────── 7-Stage Validation Pipeline ───────┐
    │  Parse → Schema → Semantic → Safety →     │
    │  Preflight → Execute → Commit             │
    └───────────────────┬───────────────────────┘
                        ↓
            ✅ Clean Commit  |  🔄 Atomic Rollback
```

| Metric | Value |
|--------|-------|
| 🟢 Unsafe state transitions | **0** across 13 production phases |
| ⚙️ Engines orchestrated | **9** independent, zero cross-talk |
| 🔄 Failure mode | **Atomic rollback** — clean commit or full revert |

---

### ⚡ [Ultra-Low Latency Order Book Engine](https://github.com/poly-chinmay/order-book-engine)
> `C++` `Lock-free DS` `Memory Pool Allocators` `SIMD`

Lock-free limit order book matching engine targeting microsecond-range latency. Custom memory pool allocators, deterministic replay, latency histogram vs naive STL.

---

### 🧠 [LLaMA-2-7B Supply Chain Fine-tune — AWS Deployed](https://github.com/poly-chinmay/llama2-supply-chain)
> `Python` `LoRA r=8` `LLaMA-2-7B` `AWS Lambda` `API Gateway`

| Metric | Before | After |
|--------|--------|-------|
| Task accuracy | 61% | **84%** |
| Inference latency | baseline | **↓22%** post-quantization |
| Deployment | — | **Production REST API on AWS** |

---

### ⚖️ [Mistral-7B — Indian Legal Judgment Summarization](https://github.com/poly-chinmay/mistral-7b-legal-india)
> `Python` `LoRA r=16` `Mistral-7B-Instruct` `A100 40GB`

| ROUGE-L | Hallucination Rate | Human Factual Accuracy |
|---------|-------------------|----------------------|
| 0.41 → **0.63** | **↓28%** | 62% → **85%** |

---

### 📈 [Reinforcement Learning Market Maker](https://github.com/poly-chinmay/rl-market-maker)
> `Python` `DQN` `Reward Shaping` `Custom LOB Simulator`

| Sharpe Ratio | Max Drawdown | Inventory Risk Variance |
|-------------|-------------|------------------------|
| 0.8 → **1.9** | **↓17%** | **↓31%** |

---

### ⚙️ [AI Inference Engine — Pure C++](https://github.com/poly-chinmay/ai-inference-cpp)
> `C++` `SIMD AVX2` `Manual Tensor Ops` · Zero external dependencies

Transformer forward pass from scratch. No PyTorch. SIMD-optimised matmul benchmarked vs PyTorch CPU.

---

## 📊 By the Numbers

<div align="center">

![](https://img.shields.io/badge/Projects_Built-20+-4f6ef7?style=for-the-badge&labelColor=0a0a0f)
![](https://img.shields.io/badge/LLMs_Fine--tuned-4-7c3aed?style=for-the-badge&labelColor=0a0a0f)
![](https://img.shields.io/badge/Best_Sharpe_Ratio-1.9-10b981?style=for-the-badge&labelColor=0a0a0f)
![](https://img.shields.io/badge/Production_Sites-3+-f59e0b?style=for-the-badge&labelColor=0a0a0f)
![](https://img.shields.io/badge/Legal_Judgments_Processed-14.5k-ef4444?style=for-the-badge&labelColor=0a0a0f)
![](https://img.shields.io/badge/Unsafe_AI_State_Transitions-0-brightgreen?style=for-the-badge&labelColor=0a0a0f)

</div>

---

## 🌐 Production

| Project | Stack | Live |
|---------|-------|------|
| DPMUN 2026 Conference Platform | Next.js · Custom Backend · Payment Gateway | [dpmun.in](https://dpmun.in) |
| Personal Site | — | [chinmayaswale.com](https://chinmayaswale.com) |

---

## 🎯 Currently

```python
chinmay = {
    "building"  : "Ghost.ai — hardened agentic pipeline in Rust",
    "studying"  : "CFA Level 1 — August 2026",
    "running"   : "DPMUN 2026 @ dpmun.in",
    "targeting" : "AI Infrastructure & Quant internships 2026",
    "philosophy": "constrain non-determinism, validate at every boundary"
}
```

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
