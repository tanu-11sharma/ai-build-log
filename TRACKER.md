# Tracker

Source of truth for the daily trending-AI-project automation.

## State

- Next rotation index: 0
- Used repo slugs: rag-knowledge-assistant, resume-job-matcher, multiagent-research-assistant, mcp-productivity-agent, support-guardrails-bot, nl-to-sql-agent, video-content-summarizer, inbox-triage-agent, workflow-automation-agent, ai-code-review-agent, meeting-notes-agent, ai-api-with-evals, content-moderation-guardrails, retrieval-eval-harness, market-analysis-agent-simulated, real-estate-pricing-agent, job-market-matching-agent, browser-task-agent-simulated, finance-budget-agent, doc-classifier-agent, doc-classifier-agent-v2
- Last run date: 2026-09-07

Note: on 2026-09-07, the full 20-item rotation was found to already be used on the account (including `doc-classifier-agent`, which a prior unlogged run had built without updating this file). Per the tracker's own overflow rule, today's build reused rotation item 20 (doc-classifier-agent) with a `-v2` suffix and a meaningfully different technical angle (TF-IDF + cosine-similarity classifier with keyword-fallback escalation, vs. the original's pure rule-based keyword scoring). Rotation index reset to 0 to start a fresh lap; going forward, cycle through the 20 ideas again, this time allowing "-v2" (or "-v3", etc.) suffixed variants whenever the base slug is already used.

## Idea rotation

Cycle through in order (wrap to the top when exhausted). Skip any slug already in "Used repo slugs" and move to the next one instead. If every base slug in a lap is already used, reuse the slug at the current index with a "-v2"/"-v3"/etc. suffix and a genuinely different angle, dataset, or twist.

1. rag-knowledge-assistant — RAG Q&A agent over a small document set, with cited answers
2. resume-job-matcher — AI resume/candidate-to-job matching agent with a "why this fits" rationale
3. multiagent-research-assistant — LangGraph multi-agent pipeline: planner -> searcher -> writer, produces a short research brief
4. mcp-productivity-agent — MCP-connected productivity assistant (tool-calling agent over a mock tasks/notes API)
5. support-guardrails-bot — Customer support chatbot with input/output guardrails (PII redaction, refusal on out-of-scope asks)
6. nl-to-sql-agent — Natural-language-to-SQL agent over a small sample SQLite database
7. video-content-summarizer — Long-form transcript summarizer + key-point extractor agent
8. inbox-triage-agent — Email/inbox triage & prioritization agent over a simulated inbox (sample data, no real email access)
9. workflow-automation-agent — Multi-step task/workflow automation agent (chains 3+ tool calls to complete a goal)
10. ai-code-review-agent — Automated code review agent that comments on a sample diff (style, bugs, missing tests)
11. meeting-notes-agent — Meeting transcript -> structured notes + action items extractor
12. ai-api-with-evals — A small deployed-style AI API with a lightweight eval/regression-test harness for its own outputs
13. content-moderation-guardrails — Content moderation / safety-guardrails demo (classifies and filters unsafe inputs)
14. retrieval-eval-harness — RAG retrieval evaluation harness measuring precision/recall against a small labeled query set
15. market-analysis-agent-SIMULATED — Backtest-only market analysis agent over historical sample data. NEVER real trading or live order execution — must say "simulation only" prominently in its README
16. real-estate-pricing-agent — Property price estimator agent over a sample listings dataset
17. job-market-matching-agent — Candidate/job market fit analysis agent (aggregate trend view, not individual medical/financial advice)
18. browser-task-agent-SIMULATED — Browser-automation-style agent that acts only on a small local mock HTML page bundled in the repo — never a real live website
19. finance-budget-agent — Personal budget/expense categorization agent over sample transaction data (clearly not financial advice)
20. doc-classifier-agent — Smart document classification/routing agent (sorts sample documents into categories)

## Safety rules for every project (non-negotiable)

- Never implement real trading/order execution, real medical diagnosis, or any real destructive browser/file/email action against live external systems.
- Default to synthetic/sample data. Any project touching finance, health, or legal topics must say clearly in its README that it is a non-production demo, not advice.
- No fabricated metrics, uptime numbers, or user counts anywhere (README, code comments, commit messages, or the LinkedIn post).
- Each project must actually run and pass its own tests before being pushed.

## Daily log

| Day | Date | Idea slug | Repo | LinkedIn post drafted? |
|---|---|---|---|---|
| 1 | 2026-09-03 | finance-budget-agent | [finance-budget-agent](https://github.com/tanu-11sharma/finance-budget-agent) | Yes |
| 2 | 2026-09-07 | doc-classifier-agent-v2 | [doc-classifier-agent-v2](https://github.com/tanu-11sharma/doc-classifier-agent-v2) | Yes |
