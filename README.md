# AI Build Log

A new small, working AI project every day -- hands-on exploration of the patterns currently showing up across AI engineering job listings: RAG, multi-agent orchestration (LangGraph), tool-using agents, guardrails, and evaluation.

Each entry below links to its own standalone repo with full code, tests, and a README.

## Why this exists

Daily practice building the specific patterns recruiters are screening for in 2026: retrieval-augmented generation, agentic workflows, MCP-connected tools, and deployment-grade structure (tests, Docker, honest docs) -- not just tutorials.

## Projects

| Date | Project | Idea area | Repo |
|---|---|---|---|
| 2026-08-24 | Retrieval Eval Harness | Offline RAG evaluation harness: TF-IDF retriever, precision@k/recall@k/MRR metrics implemented and unit-tested from scratch, run against a labeled query set via both a FastAPI service and a CLI report | [retrieval-eval-harness](https://github.com/tanu-11sharma/retrieval-eval-harness) |
| 2026-08-05 | Content Moderation Guardrails | Layered input/output guardrails for LLM apps: PII redaction, prompt-injection heuristics, and a category classifier resolved by an auditable policy engine that returns allow/redact/review/block with reasons | [content-moderation-guardrails](https://github.com/tanu-11sharma/content-moderation-guardrails) |
| 2026-08-02 | AI API With Evals | Support-ticket triage API shipped with its own eval harness: golden dataset, tested metric code, versioned thresholds, and a CI job that fails the build when model quality drops | [ai-api-with-evals](https://github.com/tanu-11sharma/ai-api-with-evals) |
| 2026-07-29 | Meeting Notes Agent | Rule-based agent that turns a meeting transcript into structured notes: summary, decisions, and action items with owners/due dates | [meeting-notes-agent](https://github.com/tanu-11sharma/meeting-notes-agent) |
| 2026-07-28 | AI Code Review Agent | Rule-based agent that reviews a unified diff and comments on style issues, likely bugs, security smells, and missing test coverage | [ai-code-review-agent](https://github.com/tanu-11sharma/ai-code-review-agent) |
