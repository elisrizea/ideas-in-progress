# Ideas in progress

I'm Alin Rizea, a Python/Django developer. I run a small company, DBM AI, and most of my work is LLM
features in live products: agents that real people talk to, and the tooling to test them.

This repo is where I write up ideas and projects I'm working on, from early designs to things already running in
production. Each one says what works, what the evidence is, and where it is still weak.

## Open to suggestions and collaboration

If something here overlaps with what you're building, if you see a flaw, or if you'd like to work on
one of these together, I'd like to hear from you.

- **Suggestions, questions, criticism:** open an [issue](https://github.com/elisrizea/ideas-in-progress/issues) on this repo.
- **Collaboration:** email me at alin.rizea@gmail.com or message me on
  [LinkedIn](https://www.linkedin.com/in/alin-rizea-b10368104/). A line about what you're working on helps.

## Ideas

| Idea | Status | Read |
| --- | --- | --- |
| **A goal-driven onboarding agent, and a scenario harness for tuning prompts.** An agent built to run on a cheap, non-reasoning model (gpt-4o-mini) that keeps a scored list of what it still needs and aims every question at the weakest gap; and prompt-audit, fixed scenarios with an LLM judge that catch prompt regressions before users see them. | Working paper, early results (Oct 2026) | [Web](https://elisrizea.github.io/ideas-in-progress/goal-driven-agent-and-prompt-tuning/) · [PDF](goal-driven-agent-and-prompt-tuning/goal-driven-agent-and-prompt-tuning.pdf) · [Folder](goal-driven-agent-and-prompt-tuning/) |
| **Project Truth: a Shazam for video claims.** Share a viral clip from any social app and get the original footage, what was cut, and what is wrong with each claim, with an evidence-based confidence rating and links to the same claim in other videos. Unknown clips are processed on the spot and added to the archive. | Design draft, nothing built yet (Oct 2026) | [Web](https://elisrizea.github.io/ideas-in-progress/project-truth/) · [PDF](project-truth/project-truth.pdf) · [Folder](project-truth/) |
| **Sonia: an AI shop assistant in one script tag.** A closed Shadow DOM widget that shares its panel with A2, the form helper; a catalogue search built from the shop's WooCommerce data; and product search that runs in the shopper's browser when a small host blocks datacenter IPs. | Live product, [demo](https://demo.dbm-ai.com/) (Oct 2026) | [Web](https://elisrizea.github.io/ideas-in-progress/sonia-shop-assistant/) · [PDF](sonia-shop-assistant/sonia-shop-assistant.pdf) · [Folder](sonia-shop-assistant/) |

More will be added here as they take shape.
