# A goal-driven onboarding agent, and a scenario harness for tuning prompts

**Working paper · early results** · Alin Rizea, DBM AI · October 2026

**Read it:** https://elisrizea.github.io/ideas-in-progress/goal-driven-agent-and-prompt-tuning/
· [PDF](goal-driven-agent-and-prompt-tuning.pdf)

## What it covers

**1. A goal-driven onboarding agent.** On Sprijin360, a directory of therapists in Romania, a practitioner
talks to an agent for a few minutes and ends with a complete public profile. The agent keeps an explicit,
scored list of nine things it still needs and aims every question at the weakest gap. It is built to run on
a small, cheap, non-reasoning model (gpt-4o-mini), so the goal and the bookkeeping live in code and the model
only does narrow language tasks. Each turn makes two
model calls (one reads the reply into scored fields, one writes the next question) with plain, tested code
in between that decides when to stop and how to break loops. At the end, a LangGraph fan-out drafts every
profile text in parallel.

**2. prompt-audit, a tool for tuning prompts.** Two Claude Code skills and a small Python harness that
replay fixed scenarios through a real LLM pipeline, snapshot every prompt with a hash, grade each answer
with a pinned LLM judge, and track score drift between runs. The paper walks through five runs on a shop
assistant where it caught a model swap that looked like a speed-up but was slower and broke a tool.

The paper also lists its current limitations, including where the method is still weak.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The paper (self-contained, served by GitHub Pages) |
| `goal-driven-agent-and-prompt-tuning.pdf` | The same paper as an A4 PDF |
| `cover.png` | Link-preview image |

The code described here lives in private repositories; this folder holds the paper only.
Suggestions and collaboration are welcome; see the [main page](../) for how to get in touch.
