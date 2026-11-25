<h1>Hi 👋🏿, I'm Blessed!</h1>

I'm a software and research engineer in Kigali, Rwanda (MS in Information Technology, Carnegie Mellon University, 2026). I build backend and data systems, and I research when AI agents give wrong answers about data, and how to catch them. Open to remote roles in backend, data and AI engineering.

<p>
  <img src="https://skillicons.dev/icons?i=python,go,ts,fastapi,postgres,redis,docker,githubactions,grafana" alt="Python, Go, TypeScript, FastAPI, PostgreSQL, Redis, Docker, GitHub Actions, Grafana">
</p>

### What I build

**Billing engine, SLS Energy (2026).** Python, FastAPI and PostgreSQL. It turns each site's daily energy readings into tariff-based PDF invoices for 9 client organisations, and it cut invoicing from 15+ days after month-end to two. Days without a meter reading are left out, never estimated.

**Infrastructure intelligence platform, MININFRA (2025).** I architected the ClickHouse pipelines and the Grafana dashboard of Rwanda's national platform for infrastructure data, built for planners and investors.

**[Sedge](https://sedge.app).** The Go backend of a text-to-SQL data platform, and its query guardrail: one read-only SELECT, allow-listed functions, a 15 s timeout and a 10,000-row cap. It blocked all 61 attack queries written to test it.

**Athletics anomaly detection (MS thesis).** A platform over 1.58M World Athletics results from 19,712 competitions (2010–2025) that compares 8 statistical and machine-learning detectors against Athletics Integrity Unit sanctions. IEEE SDS 2026, Best Paper Honorable Mention. [Paper](https://ieeexplore.ieee.org/document/11540487) · [arXiv:2604.21953](https://arxiv.org/abs/2604.21953)

Earlier: payment services in Go and TypeScript as a contract developer for Platnova and PassportMonie (2024).

### What I research

The data layer for AI agents. Before an agent writes a query, it reads definitions of what the codes and terms in the data mean. When a definition is wrong, the query still runs and the answer still looks right. I measure how often this happens and build checks that catch it.

- **Wrong definitions.** On BIRD, with two code meanings swapped in the definitions an agent reads, all 9 runs across 3 models returned the wrong count, with no warning. [Write-up](https://www.mblessed.space/blog/semantic-layer-errors)
- **Hidden rows.** Under PostgreSQL row-level security, three cheaper models presented partial answers as complete in 70–95% of affected cases. [Report](https://www.mblessed.space/blog/does-an-ai-agent-know-when-it-cannot-see-all-the-data)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/research-map-dark.svg">
  <img src="assets/research-map.svg" alt="Isometric research map of data systems for AI agents: People and agents, Agent, Meaning, Data, Definition check, Change over time and Infrastructure. An animation follows one BIRD question: two code definitions were swapped, the agent answered 22 instead of 13 with no warning, and a definition check would have caught the swap.">
</picture>

The interactive version of this map is on [my site](https://www.mblessed.space). Icons: the Isoflow isopacks (MIT, see [attribution](assets/ATTRIBUTION.txt)).

### Code

- Data agents: [agent-data-discovery-ladder](https://github.com/blessedmadukoma/agent-data-discovery-ladder) · [inside-an-llm-based-data-agent](https://github.com/blessedmadukoma/inside-an-llm-based-data-agent)
- Earlier study, on whether data agents' logs show what actually ran: [data-agent-traces](https://github.com/blessedmadukoma/data-agent-traces)
- Tools: [comment-ratchet](https://github.com/blessedmadukoma/comment-ratchet) · [go-zeptomail](https://github.com/blessedmadukoma/go-zeptomail) · [golang-web-auth](https://github.com/blessedmadukoma/golang-web-auth) · [next-go-boilerplate](https://github.com/blessedmadukoma/next-go-boilerplate) · [portfolio](https://github.com/blessedmadukoma/portfolio)

### Contact

[mblessed.space](https://www.mblessed.space) · [LinkedIn](https://www.linkedin.com/in/blessed-madukoma) · [blessedmadukoma@gmail.com](mailto:blessedmadukoma@gmail.com)

Outside work, I read, play volleyball, and follow athletics closely enough that it became a research project.
