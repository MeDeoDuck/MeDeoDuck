<div style="text-align: left;">
<h2 style="border-bottom: 1px solid #21262d; color: #c9d1d9;">
🚀 JaeHyunKim — AI Engineering Student & Research Developer
</h2>
<div style="font-weight: 700; font-size: 15px; color: #c9d1d9;">
<ul>
<li>Majoring in Artificial Intelligence Engineering at Inha University</li>
<li>Researching model compression, efficient training, and LLM-based agent systems</li>
<li>Patent holder in efficient deep learning training (Stable Diffusion + Ladder Side Tuning)</li>
</ul>
</div>
</div>

---

<div style="text-align: left;">
<h2 style="border-bottom: 1px solid #21262d; color: #c9d1d9;">
🛠️ Tech Stack
</h2>
<div align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=C%2B%2B&logoColor=white">
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white">
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black">
<img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white">
<img src="https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white">
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white">
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white">
</div>
</div>

---

<div style="text-align: left;">
<h2 style="border-bottom: 1px solid #21262d; color: #c9d1d9;">
🔬 Research & Projects
</h2>

### 🗜️ LG EXAONE 4.0 1.2B — Model Compression Pipeline
> *Compression pipeline for on-device / edge deployment of a Korean LLM*

Designed and implemented a multi-stage compression pipeline for LG's EXAONE 4.0 1.2B model, targeting significant parameter and memory reduction while preserving task performance.

- **Stage 1 — Structured Compression (choice of two approaches):**
  - **(A) 2:4 Structured Sparsity** via `llm-compressor`: enforces NVIDIA's N:M sparsity pattern, enabling hardware-accelerated sparse inference on Ampere+ GPUs
  - **(B) Depth Pruning**: surgically removes 4 transformer layers based on importance scoring, directly reducing model depth and inference latency
- **Stage 2 — Knowledge Distillation**: recovers accuracy lost during structural compression by distilling from the original EXAONE 4.0 teacher model
- **Stage 3 — GPTQ Quantization**: applies post-training quantization (4-bit) via `llm-compressor` / `auto-gptq` for final deployment-ready model size reduction

**Key tools:** `llm-compressor`, `auto-gptq`, `transformers`, PyTorch

---

### 🎨 Stable Diffusion — Ladder Side Tuning (LST) Adapter Integration
> *Patent pending — examination expected to close May 2025*

Integrated a **Ladder Side Tuning (LST)** adapter module into the Stable Diffusion training pipeline to improve fine-tuning efficiency. LST attaches a lightweight side network to frozen backbone layers, propagating gradients only through the adapter ladder rather than the full U-Net, significantly reducing GPU memory usage and training time compared to standard fine-tuning or LoRA.

- Implemented custom `forward()` hook injection to attach LST modules without modifying the original SD codebase
- Validated training efficiency gains (memory & step-time) against LoRA and full fine-tuning baselines
- Filed patent on the integration methodology *(patent under examination)*

**Key tools:** `diffusers`, PyTorch, custom CUDA hooks

---

### 🤖 YouTube Comment Filtering Agent
> *Multi-agent pipeline for intelligent comment curation with sentiment analysis*

Built a 7-step LLM-powered agent pipeline that processes raw YouTube comments into a curated, sentiment-labeled set for downstream analytics.

```
video_id list
    │
    ▼  [NUM_WORKERS = K parallel workers]
[Step 1] Raw comment collection  ──►  [Step 2] Null & duplicate removal
    │
    ▼
[Step 3] DB storage + Rule-based Soft Filter
    │
    ├── is_passed == False ──► DB only (excluded from further processing)
    │
    └── is_passed == True
            │
            ▼
      [Step 4] Candidate scoring → Top 300
            │
            ▼
      [Step 5] Multi-Criteria selection (6 criteria × Top 30 each)
            │
            ├── hit_count == 1 ──► check existence → supplement by secondary_score
            │                      secondary_score = normalized_like + normalized_reply + keyword_hits
            │
            └── hit_count >= 2 ──► [Step 6] LLM Batch Classification (parallel)
                                        │
                                        ▼
                                  [Step 7] Agent Decision Engine
                                        │
                              ┌─────────┴─────────┐
                              ▼                   ▼
                           ABSA                EXCLUDE
                   (Aspect-Based Sentiment   (filter out)
                    Analysis: POS/NEU/NEG)
                              │
                              ▼
                    [Final] Selected Comments
                            with Sentiments
```

- **`NUM_WORKERS = K`**: parallelized API call workers using async/threading to minimize LLM call latency
- **ABSA (Aspect-Based Sentiment Analysis)**: classifies retained comments with fine-grained sentiment labels per aspect
- **Agent Decision Engine**: coordinates Step 5 multi-criteria output + Step 6 LLM classification results to make final include/exclude decisions

**Key tools:** Python `asyncio`, LLM API (batch mode), custom scoring pipeline

</div>

---

<div style="text-align: left;">
<h2 style="border-bottom: 1px solid #21262d; color: #c9d1d9;">
🔭 Research Interests
</h2>
<div style="font-weight: 700; font-size: 15px; color: #c9d1d9;">
<ul>
<li>Model compression: quantization (GPTQ, AWQ), structured pruning, N:M sparsity</li>
<li>Knowledge distillation and post-training optimization for edge deployment</li>
<li>Parameter-efficient fine-tuning (LoRA, LST, adapter methods)</li>
<li>LLM-based multi-agent systems and agentic pipeline design</li>
<li>Generative model training efficiency (Stable Diffusion, Diffusion Transformers)</li>
</ul>
</div>
</div>

---

<div style="text-align: left;">
<h2 style="border-bottom: 1px solid #21262d; color: #c9d1d9;">
🧑‍💻 Contact
</h2>
<div align="center">
<a href="mailto:seankim0824@inha.edu">
<img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=Gmail&logoColor=white">
</a>
</div>
</div>

<a href="https://github.com/devxb/gitanimals">
  <img src="https://render.gitanimals.org/farms/MeDeoDuck"/>
</a>
