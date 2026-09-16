# AI Build Log

A new small, working AI project every day -- hands-on exploration of the patterns currently showing up across AI engineering job listings: RAG, multi-agent orchestration (LangGraph), tool-using agents, guardrails, and evaluation.

Each entry below links to its own standalone repo with full code, tests, and a README.

## Why this exists

Daily practice building the specific patterns recruiters are screening for in 2026: retrieval-augmented generation, agentic workflows, MCP-connected tools, and deployment-grade structure (tests, Docker, honest docs) -- not just tutorials.

## Projects

| Date | Project | Idea area | Repo |
|---|---|---|---|
| 2026-09-16 | Multi-Agent Research Assistant v2 | Agentic AI / multi-agent orchestration, v2 twist: LangGraph planner-searcher-writer-critic pipeline with a grounding-check reflection loop that revises weakly-cited sections before approving the brief | [multiagent-research-assistant-v2](https://github.com/tanu-11sharma/multiagent-research-assistant-v2) |
| 2026-09-16 | RAG Knowledge Assistant v4 | Retrieval-augmented Q&A, v4 twist: two-stage TF-IDF retrieval (document-level ranking, then sentence-level snippet extraction) for precise citations, over a synthetic cloud-storage product knowledge base | [rag-knowledge-assistant-v4](https://github.com/tanu-11sharma/rag-knowledge-assistant-v4) |
| 2026-09-11 | Resume/Job Matcher v2 | Candidate-to-job matching, v2 twist: batch many-to-many ranking (rank every candidate against a job or vice versa) with a weighted, explainable per-criterion score breakdown and explicit skill-gap output, exposed via FastAPI | [resume-job-matcher-v2](https://github.com/tanu-11sharma/resume-job-matcher-v2) |
