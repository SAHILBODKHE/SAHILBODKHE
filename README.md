# Sahil Bodkhe

**AI Engineer · Agentic AI, RAG, Agent Memory, Evaluation · Waterloo, Canada**

I build production agentic AI end to end, from the data underneath to the agents on top: multi-agent orchestration, retrieval (RAG), long-term agent memory, and evaluation that keeps model output verifiable.

In the last 1.5 years I have designed and shipped six production AI systems as sole or lead engineer, serving multiple client organisations and data at billion-row scale.

---

## Experience

### Machine Learning Engineer, Agentiiv (Dec 2025 – Nov 2026)

- Scaled the AI data product's ingestion on AWS, then Databricks: 939M rows landed from a client's 1,117-file, 275 GB archive with zero failed files, after a scan redesign that ran ~65x faster.
- Architected a long-term memory service for AI agents: per-message fact extraction, write-time deduplication that retires outdated facts, and consolidation into per-scope summaries with a relationship graph (conversation, agent, project, user).
- Built context-window management for long chats: token-pressure trimming of older turns, replaced by thread summaries served in ~200 ms on every later turn.
- Delivered on-demand memory retrieval as an agent tool: parallel search across four scopes, summary- and graph-first lookup, vector search and an LLM relevance gate with confidence scoring; zero cross-client leaks and zero invented answers on a 400-message, three-client soak test.
- Built the agentic RAG service behind the platform's Knowledge Hub: ingestion of 25+ file formats, content-aware chunking, hybrid keyword and vector search, a model-driven retrieve, rewrite, verify and retry loop, and answers cited to file and page.
- Built the multi-agent orchestration engine behind the platform's org-wide orchestrator, live for six client organisations: specialist agents exposed as tools, parallel delegation, per-conversation state and result synthesis across OpenAI, Claude and Gemini models.
- Hardened agent execution for production: concurrency limits, timeouts and cancellation that abort the in-flight model request and its cost, and structured failure results so partial answers still complete; zero resource leaks across live load tests.
- Built evaluation into the product: a QA agent that recomputes key figures before results are shown, a citation checker (Link Verifier) at 98.7% precision, and side-by-side model evaluation across Claude, Gemini and Kimi with automatic vendor fallback.
- Built real-time, reversible PII redaction for in-chat use: low-latency, cost-efficient detection with NER models (10–30 ms) and an LLM call only for doubtful cases, with custom rules for multi-PII combinations and new entity types across 25 types of personal and secret data.
- Built AI guardrails around it: per-client data isolation and user consent before any AI-made data change.
- Designed an MCP gateway giving agents a single secured, audited route to organisational tools and data.

*Python, Node.js, FastAPI · Claude, OpenAI, Gemini, MCP · embeddings, vector and hybrid search · GCP (Vertex AI), AWS, Azure · Databricks, PostgreSQL, Redis · Opik · Docker, GitHub Actions*

### Machine Learning Associate, Vector Institute (Aug 2025 – Dec 2025)

- Built a multi-agent grant-application assistant: a supervisor agent routing to research, onboarding, matching, drafting and memory specialists across 7 agents and 50+ tools; cut application effort by about 80%.
- Built an automated evaluation framework: LLM-as-a-judge scoring of every interaction on 7 factors (tool use, state, retrieval, faithfulness, routing, reasoning, memory) with evidence and suggested fixes; reduced hallucination to about 1% and API cost by 40% on conversational turns.
- Designed an early agent memory layer: retrieval from conversation, summarised memory and uploaded files before each run, with compression of older turns into memory blocks; cut token usage by 45% and model cost by 80%.

*Google ADK · LLM-as-a-judge evaluation · MongoDB, FAISS*

### GenAI Developer, Verdant InfoTech (Jul 2025 – Aug 2025)

- Delivered a plug-and-play natural-language data copilot with no fine-tuning: 85% Text-to-SQL accuracy through schema-aware retrieval, and deterministic API and SQL mapping that cut LLM output variability by 95%.

---

## Projects

**Agentic Insurance Claim Assistant** (LangGraph, MCP, LLaMA 3.2, ChromaDB, FastAPI)
Locally hosted assistant with 25+ tools behind an MCP layer; ~84% SQL accuracy and ~85% QnA precision on a 51-query benchmark using hybrid vector and graph Text-to-SQL.

**Commentary Event Decoder** (Bi-LSTM, LightGBM)
Classifies cricket events from ball-by-ball commentary without keyword rules; 86% accuracy. [Research paper](https://doi.org/10.21203/rs.3.rs-5712957/v1)

**Tim Hortons Cup Detection** (YOLOv5/v8, Optuna, MLflow, DVC, AWS EC2)
Full ML lifecycle on 4K+ images: 98.91% mAP50-95 (12% over baseline) and 22% fewer false positives, with experiment tracking, CI/CD and live monitoring.

---

## Education

- **MEng, Systems Design Engineering (AI & ML)**, University of Waterloo, 2024–2025. GPA 4.0. Certificate in Business, Conrad School.
- **BE, AI & Data Science**, University of Mumbai, 2020–2024. 9.55/10, Rank 1 in 2022 and 2024, Honors in Blockchain.

---

## Contact

sahilbodkhe45@gmail.com · [LinkedIn](https://linkedin.com/in/sahil-bodkhe-b52448197) · Waterloo, Ontario
