<h1>Hi 👋🏿, I'm Blessed!</h1>

<p>
  <b>Research and Software Engineer: AI-generated Workloads · Data Systems · Research Engineering</b><br/>
  I build data systems and study the infrastructure needed to run AI-generated workloads reliably.
</p>

<p>
  <a href="https://mblessed.space">
    <img src="https://img.shields.io/badge/Website-FFFFFF.svg?&style=for-the-badge" />
  </a>&nbsp;
  <a href="https://mblessed.space/blog">
    <img src="https://img.shields.io/badge/Blog-000000?style=for-the-badge&logo=obsidian&logoColor=white" />
  </a>&nbsp;
  <a href="https://scholar.google.com/citations?user=r2TGbRkAAAAJ&hl=en">
    <img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" />
  </a>&nbsp;
  <a href="https://www.linkedin.com/in/blessedmadukoma/">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>&nbsp;
  <a href="mailto:blessedmadukoma@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

---

### About

I am a software engineer and systems researcher studying **infrastructure for reliable AI-generated workloads**, from one-off programs to multi-step pipelines that work with tabular and other data.

My current research asks:

> How can a system derive and check the data requirements of short-lived Python programs over tabular data before an AI agent runs them?

Building my athletics anomaly-detection system required tracing each detected anomaly to its source records so I could verify the result. This showed me that reliable outputs depend on valid data and led to my current work on pre-execution checks.

- 🔬 Graduate Research Associate at **Carnegie Mellon University Africa’s SaLT Lab**
- 🧪 Completed empirical pilots on agent traces, semantic monitoring, and autonomous data discovery
- 🏗 Backend engineer working mainly with **Go** and **Python**
- 📊 Builder of data, analytics, and research infrastructure
- 🎓 **MSc Information Technology**, Carnegie Mellon University
- 🚀 Building [**Sedge**](https://sedge.app), a data workspace for context-aware analysis
- ✍🏿 Writing about research results, failed experiments, software, and data systems at [mblessed.space](https://mblessed.space)

---

### Current research

I am studying whether exact data checks can detect failures before agent-generated programs run.

I have completed an initial study of [DuckDQ](https://ssc.io/pdf/duckdq.pdf) and [PrismaDV](https://arxiv.org/abs/2604.21765). My next step is to inspect failed and successful DABstep executions, classify their failure causes, and test whether a justified pre-execution check could detect a real source-data failure.

In parallel, I am prototyping schema-aware validation for generated SQL in Sedge using [GoSQLX](https://github.com/ajitpratap0/GoSQLX).

---

### Research publications

**Performance Anomaly Detection in Athletics: A Benchmarking System with Visual Analytics**  
Blessed Madukoma and Prasenjit Mitra. IEEE Swiss Conference on Data Science and AI, 2026.  
🏅 *Honorable Mention, Best Full Paper.*

[Paper](https://ieeexplore.ieee.org/document/11540487) · [arXiv](https://arxiv.org/abs/2604.21953) · [Live system](https://athletics-performance.mblessed.space)

**Unmasking COVID-19 Vulnerability in Nigeria: Mapping Risks Beyond Urban Hotspots**  
Sheila Wafula and Blessed Madukoma. Women in Machine Learning Workshop at NeurIPS 2025.

[Workshop](https://neurips.cc/virtual/2025/loc/san-diego/133847) · [arXiv](https://arxiv.org/abs/2509.05398)

---

### Selected research experiments

**[Can an AI Agent Find Its Own Data?](https://mblessed.space/blog/can-an-ai-agent-find-its-own-data)**  
Tested three models on 33 questions under two conditions: with the relevant files isolated and with the same files hidden inside a corpus of 7,985 documents. The experiment also exposed five errors in my evaluation harness.

**[Semantic Monitoring Under AI Component Evolution](https://mblessed.space/blog/can-safety-checker-trust-changed-ai-extractor)**  
Tested how a structurally valid output from a changed AI component can cause an unchanged downstream safety checker to make a false-safe decision.

---

### Selected engineering work

**[Sedge](https://sedge.app)**  
Building a data workspace that combines natural-language and SQL analysis with schema and metadata context.

`Go` `SQL` `PostgreSQL`

**[Athletics Performance Anomaly Detection](https://athletics-performance.mblessed.space)**  
Built a benchmarking platform over 1.5M+ track and field performances from 19,000+ competitions between 2010 and 2025. It compares 14 statistical, machine-learning, and Bayesian methods and validates detected anomalies against publicly confirmed Athletics Integrity Unit sanctions.

`Python` `FastAPI` `HTMX` `PostgreSQL` `DuckDB` `Redis` `Docker` `Ansible`

**[go-zeptomail](https://github.com/blessedmadukoma/go-zeptomail)**  
Built a native Go SDK for ZeptoMail’s transactional email API.

`Go`

---

### Tools I use

**Languages**  
![Go](https://img.shields.io/badge/-Go-29BEB0?style=for-the-badge&logo=go&logoColor=white)&nbsp;
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=FFD43B)&nbsp;
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)&nbsp;
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Backend and web**  
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)&nbsp;
![HTMX](https://img.shields.io/badge/HTMX-36C?style=for-the-badge&logo=htmx&logoColor=white)&nbsp;
![Nuxt](https://img.shields.io/badge/Nuxt-00DC82?style=for-the-badge&logo=nuxtdotjs&logoColor=white)&nbsp;
![Vue](https://img.shields.io/badge/Vue-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D)&nbsp;
![Tailwind](https://img.shields.io/badge/Tailwind-%231552B9.svg?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Data and ML**  
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)&nbsp;
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)&nbsp;
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)&nbsp;
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)&nbsp;
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)&nbsp;
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)&nbsp;
![Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)&nbsp;
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

**Storage and infrastructure**  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)&nbsp;
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)&nbsp;
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)&nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)&nbsp;
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)&nbsp;
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

**Research and writing**  
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)&nbsp;
![Overleaf](https://img.shields.io/badge/Overleaf-47A141?style=for-the-badge&logo=overleaf&logoColor=white)&nbsp;
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white)

---

### Recent writing

- 🧪 [Can an AI Agent Find Its Own Data? I Spent a Night Finding Out](https://mblessed.space/blog/can-an-ai-agent-find-its-own-data)
- 🧪 [Historical Trace Coverage for Regression Selection in Stochastic Tool-Using Agents](https://mblessed.space/blog/can-old-agent-traces-guide-regression-testing)
- 🧪 [Semantic Monitoring Under AI Component Evolution](https://mblessed.space/blog/can-safety-checker-trust-changed-ai-extractor)
- 🚫 [When the Interference Isn’t There: What a Null Result Taught Me About LLM Serving](https://mblessed.space/blog/when-the-interference-isnt-there)

Archive: [Hashnode](https://mblessed.hashnode.dev/) for posts published before May 2026.

---

### Elsewhere

Outside work, I read, play volleyball, and follow athletics closely enough that it became a research project.

<p>
  <img src="https://github-readme-stats.vercel.app/api?username=blessedmadukoma&show_icons=true&theme=tokyonight&line_height=40" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=blessedmadukoma&hide=css,java,php,blade,shell,dockerfile,html&theme=tokyonight" />
</p>

<img height="200" width="800" align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=blessedmadukoma&theme=highcontrast" alt="GitHub contribution streak" />
