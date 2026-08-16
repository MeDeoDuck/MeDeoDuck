<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2F80ED,100:141E30&height=210&section=header&text=Jaehyun%20Kim&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Continual%20Knowledge%20Editing%20·%20MoE%20%26%20Routing%20·%20Parameter-Efficient%20LLMs%20·%20Agentic%20AI&descSize=15&descAlignY=60"/>

<p align="center">
  <a href="mailto:seankim0824@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://github.com/MeDeoDuck"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>
<p align="center"><i>AI Engineering undergraduate at Inha University · AI engineer intern · seeking M.S. research</i></p>


## 👋 About me

I'm an Artificial Intelligence Engineering undergraduate at Inha University (GPA 4.10/4.50, expected graduation Feb 2027) and an AI engineer intern, with hands-on work in **knowledge distillation, parameter-efficient adaptation, agentic AI, and multimodal learning**.

I treat an LLM as a component to engineer around, not to trust blindly — which is also what pulls me toward research. Both directions I care about come from the same question: *how do you add knowledge to a model without breaking what it already knows?* I want to answer it with **continual knowledge editing** and **query-aware routing of parameter-efficient expert modules** over a shared frozen backbone.

<br>

## 🔬 Research Interests

- **Continual Knowledge Editing** — learning continually arriving knowledge without repeated parameter updating or merging
- **Mixture-of-Experts & Query-Aware Routing** — routing at the *module* level rather than selecting between whole models
- **Parameter-Efficient LLM Adaptation** — LST-inspired side modules over a frozen backbone
- **Agentic AI** — multi-agent orchestration, verification gates, and reliability under repeated runs

### Proposed direction

> **Research question.** Can continually arriving knowledge be learned in parameter-efficient side modules and selectively composed with a shared frozen LLM, reducing the interference caused by repeated parameter updating or merging?

| | Pipeline |
|---|---|
| **SeqMMR** (motivating work) | Query → unedited backup / merged edited model |
| **Proposed** | Query → hybrid knowledge router → frozen LLM + selected LST-inspired module(s) → response |

Two open questions I want to attack: whether **semantic relevance alone is a sufficient routing signal** (or whether entity–relation structure and query context should complement it), and whether edit-relevant knowledge can be routed at **module granularity**. Planned evaluation axes: edit success & retention, routing accuracy, locality & module interference, and incremental efficiency.

<br>

## ⚒️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white"/>
</p>

- **Programming & ML:** Python, PyTorch, Hugging Face Transformers, NumPy / pandas / scikit-learn
- **Model adaptation:** knowledge distillation, Ladder Side-Tuning, PEFT, quantization (GPTQ / AWQ)
- **Agent systems:** LangGraph, LangChain, verification-gate / guardrail design, multi-agent orchestration
- **Multimodal AI:** latent diffusion, VLMs, object detection, tracking, ReID
- **Graphs & time series:** PyTorch Geometric (GAT / GCN / GraphSAGE), forecasting (PatchTST, DLinear, iTransformer)
- **Systems & robotics:** FastAPI, PostgreSQL, Docker, CUDA, ROS, C++

**Tools**

<p align="center">
  <img src="https://img.shields.io/badge/Anaconda-44A833?style=flat-square&logo=anaconda&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyCharm-000000?style=flat-square&logo=pycharm&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Weights%20%26%20Biases-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black"/>
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Overleaf-47A141?style=flat-square&logo=overleaf&logoColor=white"/>
  <img src="https://img.shields.io/badge/LaTeX-008080?style=flat-square&logo=latex&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
</p>

<br>

## 🔥 Featured Projects

<table>
  <thead>
    <tr><th>Project</th><th>What it is</th><th>Result</th><th>Links</th></tr>
  </thead>
  <tbody>
    <tr>
      <td><b>MOABOM</b><br/><sub>Knowledge Distillation · Agentic AI<br/>Mar – Jun 2026</sub></td>
      <td>Multi-agent system that synthesizes scattered YouTube tech reviews into one structured 7-section purchase-decision report. A LangGraph supervisor routes execution on DB state — cache retrieval, autonomous data enrichment, or full report generation — over video-selection, comment-filtering, and report-writer agents, with cross-model verification against source bias.</td>
      <td><b>Distillation:</b> replaced GPT-4.1 comment classification (6,375 teacher-labeled samples) and comparison-video classification (1,776 samples) with locally deployed KLUE-based models — <b>22× lower end-to-end inference latency</b>, API calls eliminated for the replaced stage, ~60 ms per-video pre-filtering.<br/><b>Reliability:</b> <b>98% judgment consistency</b> over 300 trials (3 models × 10 products × 10 repetitions), above GPT-4.1 (90%) and Gemini (86%).<br/><b>Deployment:</b> shipped and evaluated with 97 users over roughly a one-week deployment-and-survey period; cuts product research from 120 min to under 5 min.</td>
      <td><a href="https://github.com/moabom-official/Moabom_Prototype">Repo</a> · <a href="https://github.com/MeDeoDuck/KLUE_BERT_DISTILL">Distillation</a> · <a href="https://github.com/MeDeoDuck/MoabomVSAll">Benchmark</a></td>
    </tr>
    <tr>
      <td><b>FOMO Breaker</b><br/><sub>Multi-Agent Systems · Evidence Verification<br/>Jun – Jul 2026</sub></td>
      <td>Multi-agent debate system that checks whether a stock urge is analysis or FOMO. Five persona agents, each grounded in a different economic or behavioral-finance theory with its own risk threshold and time horizon, deliberately reach different conclusions from the same market data; the free-form debate is structured into a FOMO-index dashboard. A second-opinion tool, not a recommender.</td>
      <td><b>Verification gate:</b> supporting evidence is validated for accuracy and weight adjustments are checked against predefined bounds in code — <b>294 of 736 generated statements</b> were withheld or rejected for regeneration.<br/><b>Consistency:</b> <b>96.7%</b> (29 of 30 runs matched) under frozen inputs; issued cautionary calls on 5 of 6 stocks, the most risk-sensitive of the systems compared.<br/><b>Dual-LLM channel separation:</b> persona speech (GPT-4.1 / Llama-3.3-70B, temp 0.7) split from moderator summarization (Llama-3.3-70B via Groq, temp 0.3), so confidence scores are computed only from the persona channel and a cheap summarizer can't distort reliability. Channel-specific timeouts and rule-based fallbacks keep the debate alive when a call fails.</td>
      <td><a href="https://github.com/FOMO-Breaker/FOMO-Breaker">Repo</a> · <a href="https://fomo-breaker.vercel.app">Live demo</a></td>
    </tr>
    <tr>
      <td><b>Latent Diffusion + Ladder Side-Tuning</b><br/><sub>PEFT · Modular Adaptation<br/>Jul – Aug 2025</sub></td>
      <td>Parameter-efficient adaptation of a Latent Diffusion U-Net: LST side modules are integrated into each U-Net block during denoising, taking block intermediate features concatenated with the previous LST output, while the backbone stays frozen and gradients never propagate through it. Only the side network and ladder connections are trained.</td>
      <td>On LSUN Churches (192×192, TITAN RTX): GPU memory <b>23,115 → 16,509 MiB (−28.6%)</b> and training time <b>1h 07m 08s → 32m 12s (2.08× speedup)</b> vs. full fine-tuning. Limitation: efficiency-only evaluation so far — generation-quality preservation is still to be measured. This project is what led to the routing direction above: independently trained expert modules composed over one shared frozen backbone.<br/><i>Registered software copyright; source kept private.</i></td>
      <td><a href="https://github.com/MeDeoDuck/StableDiffusionWithLST">Repo</a></td>
    </tr>
  </tbody>
</table>

## 🧩 Other Projects

- **[CAGE-CareRF](https://github.com/ITDA-Team-C/FINAL_GNN_STRUCTURE)** — multi-relation GNN that catches organized fake-review rings by modeling reviews as a 6-relation graph (+7.4% PR-AUC over GNN baselines). `PyTorch Geometric · GAT / GCN / GraphSAGE · SBERT`
- **[ShiftLoss](https://github.com/MeDeoDuck/ShiftLoss)** — adds a differentiable time-delay term to [DBLoss](https://arxiv.org/abs/2510.14510) (NeurIPS 2025) so time-series forecasts tolerate small phase offsets; research paper under review. `Amplifier · PatchTST · DLinear · iTransformer`
- **[LG Aimers (quantization)](https://github.com/MeDeoDuck/LG_Aimers_8th_Quant)** — LLM compression experiments for cheaper inference. `GPTQ · AWQ · sparsity`
- **[TrackWithReID](https://github.com/MeDeoDuck/TrackWithReID)** — multi-object tracking with re-identification. `YOLOX · ByteTrack · TransReID (ViT) · OpenCV`
- **[VoiceStep](https://github.com/MeDeoDuck/VoiceStep)** — AI voice-conversation practice for job interviews and workplace communication (speech in, LLM agent, spoken reply). `FastAPI · faster-whisper · Gemini · React`
- **[Linkus20 Agent Editor](https://github.com/MeDeoDuck/Linkus20-AgentStructureEducation)** — block-diagram editor with an LLM agent that builds and edits diagrams from natural language. `React · TypeScript · Express · LLM`
- **[Physical_AI_ws](https://github.com/MeDeoDuck/Physical_AI_ws)** — CCTV perception → A* planning → Pure Pursuit control, a warehouse-robot pipeline. `ROS · Python`
- **[Lider_Cone_Path](https://github.com/MeDeoDuck/Lider_Cone_Path)** — LiDAR cone-detection and path planning written from scratch, including Hungarian matching. `C++`
- **[desktop-planner](https://github.com/MeDeoDuck/desktop-planner)** — minimal desktop planner app. `Electron · JavaScript`

<br>

## 🐢 Experience & Education

**GeoAI Group Intern**, Wavus — Jul 2026 ~ Present
- Independently planned and implemented three scenario-specific disaster-prevention AI systems for a WSCE exhibition booth: dam water-level monitoring (Tesseract + Qwen), indoor fire-risk prediction (YOLOX + SlowFast + Qwen), and crowd-risk prediction (YOLOX + Qwen)
- Built exhibition-ready monitoring pipelines integrating OCR, object detection, video understanding, and VLM-based scene interpretation with real-time risk visualization and alert generation

**B.S. in Artificial Intelligence Engineering**, Inha University — Mar 2021 ~ Present
- Expected graduation Feb 2027 · GPA 4.10/4.50
- Undergraduate Researcher: Financial AI Lab (Dec 2025 ~ Jun 2026) · Vision and Learning Lab (Jun 2025 ~ Oct 2025) · Autonomous Systems Lab (Mar 2025 ~ Jun 2025)

**Other activities**

| Period | Activity | Role |
|---|---|---|
| Jul 2026 ~ Present | **LinkUs** (AI talent network), 20th | Vice President — leading the rebrand from a career-networking group into an AI talent network, as the only engineer on the leadership team |
| Mar ~ Jun 2025 | **LinkUs**, 19th | Member |
| Jan ~ Feb 2026 | **LG Aimers 8th** (LG AI training program) | LLM Compression track, completed with certificate |
| Mar 2025 ~ Feb 2026 | Future Automotive Engineering Dept, Inha University | Student Ambassador |

<br>

## 🏆 Awards & Registrations

| Date | Award / Registration | Detail | Host |
|---|---|---|---|
| Jun 2026 | 🥈 **Excellence Award** | Dean's Award, College of Software and Convergence | Inha University |
| Nov 2024 | 🏆 **Grand Prize** | LINC 3.0 Project Group Director's Award | Inha University |
| 2026 | 🏆 **Grand Prize** | LinkUs Club Activity Award | LinkUs |
| Jul 2026 | 📄 **Software Copyright** `C-2026-03297` | MOABOM | KCC |
| May 2026 | 📄 **Software Copyright** `C-2026-022267` | Stable Diffusion Training Enhancement Program Based on Ladder Side-Tuning | KCC |

**Certifications** — OPIc IH (English) · SQLD

<p align="center">Currently seeking <b>M.S. research on continual knowledge editing and query-aware routing of parameter-efficient expert modules</b>.<br/>The fastest way to judge me is MOABOM, <a href="https://fomo-breaker.vercel.app">FOMO Breaker</a>, and the LST work above. Reach me at seankim0824@gmail.com</p>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:141E30,100:2F80ED&height=100&section=footer"/>
