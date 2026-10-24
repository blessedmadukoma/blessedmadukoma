<h1>Hi 👋🏿, I'm Blessed!</h1>

<p>
  <b>Software &amp; Research Engineer · LLM agents and AI data systems</b><br/>
  I study how to keep AI-powered data systems correct as data, definitions, access rules and tools change, and what that costs.
</p>

<p>
  <a href="https://mblessed.space">
    <img src="https://img.shields.io/badge/Website-FFFFFF.svg?&style=for-the-badge" />
  </a>&nbsp;
  <a href="https://www.mblessed.space/docs/Madukoma%20Blessed%20Resume.pdf">
    <img src="https://img.shields.io/badge/Resume-PDF-24292F?style=for-the-badge" />
  </a>&nbsp;
  <a href="https://mblessed.space/blog">
    <img src="https://img.shields.io/badge/Blog-000000?style=for-the-badge&logo=obsidian&logoColor=white" />
  </a>&nbsp;
  <a href="https://scholar.google.com/citations?user=r2TGbRkAAAAJ&hl=en">
    <img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" />
  </a>&nbsp;
  <a href="https://www.linkedin.com/in/blessed-madukoma/">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>&nbsp;
  <a href="mailto:blessedmadukoma@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

---

### About

I am a software engineer and researcher: building AI agents and data systems, and studying **the errors that make their answers wrong without anyone noticing**. A correct answer matches complete, up-to-date data, or it says clearly that it is incomplete.

My current research asks:

> When something an answer depends on changes, which answers become wrong, and what is the cheapest way to fix or flag them?

Building my athletics anomaly-detection system required tracing each flag to its source records so investigators could check it: a flag is a lead, not a verdict. AI agents need the same rule. People act on what a data system reports, so the system must show what its answer rests on.

- 🧪 Studied AI agents that write code to analyse data: [what their traces do not record](https://github.com/blessedmadukoma/data-agent-traces) and [whether they know when they cannot see all the data](https://www.mblessed.space/blog/does-an-ai-agent-know-when-it-cannot-see-all-the-data)
- 🤖 Building a Fantasy Premier League agent with traces and evals, used by five testers
- 🏗 Backend engineer working mainly with **Go** and **Python**; most recently built a metered billing engine at SLS Energy
- 📊 Built data pipelines and a Grafana dashboard of 12+ indicators for Rwanda's Ministry of Infrastructure
- 🎓 **MSc Information Technology**, Carnegie Mellon University
- 🚀 Building [**Sedge**](https://sedge.app), a data operating system that uses AI to answer questions about a company's data
- ✍🏿 Writing about research results, failed experiments, software, and data systems at [mblessed.space](https://mblessed.space)

---

### What I have found

With Prof. Prasenjit Mitra at CMU Africa's SaLT Lab, I studied AI agents that write code to analyse data.

- **Logs can blame the model for the software around it.** In DataAgentBench's public logs, that software caused 37% of the recorded failures (16,293 of 44,277; 21.6% of all code steps), and the logs showed these failures as the model's own. Removing them changed how six models ranked ([code](https://github.com/blessedmadukoma/data-agent-traces)).
- **Errors the model can see are the smaller problem.** Across 36,990 pre-registered runs, a checker that stops code from using columns or files that do not exist cut the number of these errors that reached execution from 3,316 to 2 for gpt-oss-120b, but raised accuracy by only 0.68 points. A clear error message worked as well.
- **Errors the model cannot see stay silent.** When access rules hid some rows and the model was not told, cheaper models presented incomplete answers as complete in 70–95% of affected cases ([study](https://www.mblessed.space/blog/does-an-ai-agent-know-when-it-cannot-see-all-the-data)).

Better models will keep fixing errors they can see. They cannot fix what the data does not show, such as a definition that changed or rows they may not read. My Fantasy Premier League agent once reported the wrong scores for a footballer while its log showed a successful step.

I am now working on the question above in [Sedge](https://sedge.app).

---

### Research publications

**Performance Anomaly Detection in Athletics: A Benchmarking System with Visual Analytics**  
Blessed Madukoma and Prasenjit Mitra. IEEE Swiss Conference on Data Science and AI, 2026.  
🏅 *Honorable Mention – Best Paper Award.*

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

**Metered billing engine, SLS Energy** (Jun–Aug 2026)  
Replaced a manual spreadsheet with a metered billing engine that invoices 9 client organisations: invoices now go out two days after month-end instead of over a month. Closed all 18 critical and high-severity findings in the platform, including 8 cross-tenant data-exposure flaws, and set up CI gates (pytest at 80% coverage, mypy, ruff, pip-audit, gitleaks).

`Python` `FastAPI` `PostgreSQL`

**[Athletics Performance Anomaly Detection](https://athletics-performance.mblessed.space)**  
Built a benchmarking platform over 1.6 million track and field performances from 19,000+ competitions between 2010 and 2025. It combines eight statistical, machine-learning, and Bayesian methods to narrow 31,604 athletes to about 163 for investigator review, and checks the flags against Athletics Integrity Unit sanctions. Each flag links to its evidence. Replacing a four-container Kafka pipeline with one FastAPI service cut a full analysis from 129 s to 33 s.

`Python` `FastAPI` `HTMX` `PostgreSQL` `DuckDB` `Redis` `Docker` `Ansible`

**[Sedge](https://sedge.app)**  
Building a data operating system that uses AI to answer questions about a company's data. I am adding the checks every AI-written query must pass before it runs (in code review).

`Go` `SQL` `PostgreSQL`

**[go-zeptomail](https://github.com/blessedmadukoma/go-zeptomail)**  
Built a native Go SDK for ZeptoMail’s transactional email API.

`Go`

---

### Tools I use

**Languages**  
![Go](https://img.shields.io/badge/-Go-29BEB0?style=for-the-badge&logo=go&logoColor=white)&nbsp;
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=FFD43B)&nbsp;
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)&nbsp;
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)&nbsp;
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**Backend and web**  
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)&nbsp;
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)&nbsp;
![HTMX](https://img.shields.io/badge/HTMX-36C?style=for-the-badge&logo=htmx&logoColor=white)&nbsp;
![Nuxt](https://img.shields.io/badge/Nuxt-00DC82?style=for-the-badge&logo=nuxtdotjs&logoColor=white)&nbsp;
![Vue](https://img.shields.io/badge/Vue-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D)&nbsp;
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)&nbsp;
![Tailwind](https://img.shields.io/badge/Tailwind-%231552B9.svg?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Data, ML and LLMs**  
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)&nbsp;
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)&nbsp;
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Storage, infrastructure and testing**  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)&nbsp;
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)&nbsp;
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)&nbsp;
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)&nbsp;
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)&nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)&nbsp;
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)&nbsp;
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)&nbsp;
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)&nbsp;
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)

**Research and writing**  
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)&nbsp;
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
