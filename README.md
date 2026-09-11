# AI Build Log

A new small, working AI project every day -- hands-on exploration of the patterns currently showing up across AI engineering job listings: RAG, multi-agent orchestration (LangGraph), tool-using agents, guardrails, and evaluation.

Each entry below links to its own standalone repo with full code, tests, and a README.

## Why this exists

Daily practice building the specific patterns recruiters are screening for in 2026: retrieval-augmented generation, agentic workflows, MCP-connected tools, and deployment-grade structure (tests, Docker, honest docs) -- not just tutorials.

## Projects

| Date | Project | Idea area | Repo |
|---|---|---|---|
| 2026-09-11 | Resume/Job Matcher v2 | Candidate-to-job matching, v2 twist: batch many-to-many ranking (rank every candidate against a job or vice versa) with a weighted, explainable per-criterion score breakdown and explicit skill-gap output, exposed via FastAPI | [resume-job-matcher-v2](https://github.com/tanu-11sharma/resume-job-matcher-v2) |
| 2026-09-09 | RAG Knowledge Assistant v2 | RAG Q&A agent over a synthetic SaaS FAQ knowledge base: Okapi BM25 retrieval (implemented from scratch), conversational follow-up resolution, and a low-confidence refusal gate, exposed via FastAPI | [rag-knowledge-assistant-v2](https://github.com/tanu-11sharma/rag-knowledge-assistant-v2) |
