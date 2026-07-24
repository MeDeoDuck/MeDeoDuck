<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:2F80ED,100:141E30&height=210&section=header&text=Jaehyun%20Kim&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=AI%20Engineer%20·%20LLM%20agent%20products,%20built%20to%20run%20cheap%20in%20production&descSize=17&descAlignY=60"/>

<p align="center">
  <a href="mailto:seankim0824@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://github.com/MeDeoDuck"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>
<p align="center"><i>Open to AX / generative-AI engineer roles</i></p>

## 👋 About me

I build LLM agent products and make them cheap enough to run in production. My flagship is a multi-agent service I shipped to real users, then cut its inference cost about 99%.

Backend, the agent layer, and the cost work: I take a generative-AI service the whole way, not just to a demo.

<br>

## ⚒️ Tech Stack

Only what I've actually built with, focused on generative-AI / AX work.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white"/>
  <img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logo=groq&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
</p>

- **LLM & agents:** multi-agent orchestration (LangGraph), prompt engineering, harness / guardrail engineering
- **Model efficiency:** knowledge distillation, quantization (GPTQ / AWQ)
- **ML & research:** GNN (PyTorch Geometric), time-series forecasting, PyTorch / Hugging Face
- **Computer vision & robotics:** detection and tracking (YOLOX, ByteTrack), re-identification (ViT), LiDAR, ROS, C++
- **Backend & deploy:** FastAPI, PostgreSQL, Docker, cloud deploy (Azure, Vercel)

<br>

## 🔥 Featured Projects

<table>
  <thead>
    <tr><th>Project</th><th>What it is</th><th>Result</th><th>Links</th></tr>
  </thead>
  <tbody>
    <tr>
      <td><b>Moabom</b></td>
      <td>Multi-agent LLM service that turns scattered YouTube tech reviews into one purchase-decision report. Video selection, comment filtering, and report generation run as a LangGraph agent pipeline. FastAPI + PostgreSQL, deployed on Azure.</td>
      <td>To cut API cost, distilled GPT-4.1's comment and comparison-video classification into local KLUE-RoBERTa models (macro F1 <b>0.92 / 0.90</b>), holding accuracy while running inference <b>22x faster</b> and <b>~99% cheaper</b> on a self-hosted GPU. Judgment consistency <b>98%</b> across 300 runs (GPT-4.1 90%, Gemini 86%). Deployed pilot, MAU 97.</td>
      <td><a href="https://github.com/moabom-official/Moabom_Prototype">Repo</a> · <a href="https://github.com/MeDeoDuck/KLUE_BERT_DISTILL">Distillation</a> · <a href="https://github.com/MeDeoDuck/MoabomVSAll">Benchmark</a></td>
    </tr>
    <tr>
      <td><b>FOMO Breaker</b></td>
      <td>Multi-agent debate system that checks whether a stock urge is analysis or FOMO. AI personas argue back and forth over rounds with a moderator, and the free-form debate is structured into a FOMO-index dashboard and verdict. Deployed; a second-opinion tool, not a recommender.</td>
      <td>Persona design: each agent is grounded in a different finance theory, with its own risk threshold and time horizon, so the same input yields deliberately different views. Harness engineering: every weight proposal is validated in code against the real signal scores and per-item caps, held or rejected otherwise (<b>53% held/rejected</b> over 30 runs), with zero-sum weights and an index re-derivation check. Dual-LLM: GPT-4.1 for speech, Llama-3.3-70B for internal reasoning, over WebSocket.</td>
      <td><a href="https://github.com/FOMO-Breaker/FOMO-Breaker">Repo</a> · <a href="https://fomo-breaker.vercel.app">Live demo</a></td>
    </tr>
  </tbody>
</table>

## 🧩 Other Projects

- **[VoiceStep](https://github.com/MeDeoDuck/VoiceStep)** — AI voice-conversation practice for job interviews and workplace communication (speech in, LLM agent, spoken reply). `FastAPI · faster-whisper · Gemini · React`
- **[Linkus20 Agent Editor](https://github.com/MeDeoDuck/Linkus20-AgentStructureEducation)** — block-diagram editor with an LLM agent that builds and edits diagrams from natural language. `React · TypeScript · Express · LLM`
- **[CAGE-CareRF](https://github.com/ITDA-Team-C/FINAL_GNN_STRUCTURE)** — multi-relation GNN that catches organized fake-review rings by modeling reviews as a 6-relation graph (+7.4% PR-AUC over GNN baselines). `PyTorch Geometric · GAT / GCN / GraphSAGE · SBERT`
- **[ShiftLoss](https://github.com/MeDeoDuck/ShiftLoss)** — adds a differentiable time-delay term to [DBLoss](https://arxiv.org/abs/2510.14510) (NeurIPS 2025) so time-series forecasts tolerate small phase offsets; research paper under review. `Amplifier · PatchTST · DLinear · iTransformer`
- **[LG Aimers (quantization)](https://github.com/MeDeoDuck/LG_Aimers_8th_Quant)** — model-compression experiments for cheaper inference. `GPTQ · AWQ · sparsity`
- **[TrackWithReID](https://github.com/MeDeoDuck/TrackWithReID)** — multi-object tracking with re-identification. `YOLOX · ByteTrack · TransReID (ViT) · OpenCV`
- **[Physical_AI_ws](https://github.com/MeDeoDuck/Physical_AI_ws)** — CCTV perception to A* planning to Pure Pursuit control, a warehouse-robot pipeline. `ROS · Python`
- **[Lider_Cone_Path](https://github.com/MeDeoDuck/Lider_Cone_Path)** — LiDAR cone-detection and path planning written from scratch, including Hungarian matching. `C++`
- **[desktop-planner](https://github.com/MeDeoDuck/desktop-planner)** — minimal desktop planner app. `Electron · JavaScript`

<br>

## 🐢 Experience & Education

- **Work-Study Intern**, WAVUS (GeoAI / spatial-information platform), Jul 2026 ~ Present
- **Undergraduate Researcher**, Inha University
  - Financial AI Lab (Dec 2025 ~ Aug 2026)
  - Vision & Learning Lab (Jun 2025 ~ Oct 2025)
  - Autonomous Systems Lab (Mar 2025 ~ Jun 2025)
- **B.S. in Artificial Intelligence Engineering**, Inha University (2021 ~ Present)
- **LinkUs** (AI talent network): Vice President, 20th (Jul 2026 ~ Present) · Member, 19th (Mar 2025 ~ Jun 2025). Leading the club's rebrand from a career-networking group into an AI talent network as the only engineer on the leadership team.
- **Awards:** **Capstone Design 3rd Prize, Dean's Award of the College of Software Convergence, Inha University** (2026) · Incomthon Grand Prize (LINK 3.0 Director's Award, 2024) · LinkUs Club Activity Grand Prize (2026)
- **Certifications:** OPIc IH (English) · SQLD
- **Software copyright registrations (2):** Moabom · LST-based Stable Diffusion training method

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:141E30,100:2F80ED&height=100&section=footer"/>
