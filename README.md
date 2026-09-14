# Hi, I'm Sayandip 👋

Associate Director of Product @ Zeta | 13+ yrs in product | Building credit card products (UK/US) by day, exploring cross-border payments and reg-tech by night

## What I build

- **Retrieval systems with teeth.** Intent classifiers + reranking + structure-aware chunking + page-precise citations. I treat the eval harness as part of the architecture, not an afterthought — it's the thing that lets me move retrieval quality in one direction.
- **Tooling that respects operators.** When non-engineers need to make safe changes (call flows, prompts, ticket workflows), I split the surface into "code-reviewed" and "operator-self-serve," and put real telemetry behind both.
- **Automations that work around vendor SaaS limits.** When the UI blocks something the API supports, I reach for `fetch` interception, React Fiber traversal, and coordinate clicks — not headless browsers driving the DOM.
- **AI-assisted workflows with human review gates.** Agents are most useful when they expand a grounded scope (a PRD, an AC, an existing test plan), produce a strict findings packet, and stop short of writing into systems humans care about until a person has signed off.

## Selected projects

| Repo | What it is | Stack |
|---|---|---|
| [enterprise-rag-knowledge-base](https://github.com/sayandip1987/enterprise-rag-knowledge-base) | RAG Q&A over ~2,400 chunks of internal product docs · 4.96/5.00 quality on 19-test eval · 100% in-module precision post-rerank | Next.js 14 · Qdrant · OpenAI · GPT-4o(-mini) |
| [uk-compliance-knowledge-base](https://github.com/sayandip1987/uk-compliance-knowledge-base) | RAG over the UK retail-financial-services rulebook · 16,829 chunks across 887 docs · page-precise PDF citations · cite-or-refuse discipline | Next.js 14 · Qdrant · `pdf-parse` · `cheerio` |
| [amazon-connect-flow-tools](https://github.com/sayandip1987/amazon-connect-flow-tools) | Visualise / fix / validate Amazon Connect contact flows before import — built from production fintech IVR pain. stdlib-only Python | Python 3.8+ stdlib · draw.io |
| [spa-automation-toolkit](https://github.com/sayandip1987/spa-automation-toolkit) | Browser-side patterns for automating React SPAs when the UI gets in the way — fetch interception, Fiber traversal, coordinate clicks | Vanilla JS (ES2017+) · React Fiber |
| [uat-jira-automation](https://github.com/sayandip1987/uat-jira-automation) | Agent-driven UAT bug triage + deduplication + batch Jira filing · 29 raw findings → 18 dedup-matched + 12 net-new tickets in 3 sessions | AI browser-automation agent · Atlassian Jira |

## How I think about AI first product development

A few opinions that show up in everything above:

- **Boring before clever.** Better chunking and a reranker beat HyDE and graph indexes on most corpora. Coordinate clicks beat clever DOM heuristics on Atlaskit. Reach for the fancy thing only after the boring thing has hit a measured ceiling.
- **The schema of the output is the product.** A loose "tell me what's broken" prompt produces unreviewable noise. A strict findings packet — citation, repro, evidence, confidence — produces a queue people respect.
- **Run inside the user's session.** Re-implementing SSO/MFA in a headless harness is almost always a worse use of time than borrowing a logged-in browser and being deliberate about side effects.
- **Reversibility is a feature.** Infra-as-code for things customers touch. Backups before destructive ingest. Validate-before-promote pipelines. Every project above has a "we can roll this back" story baked in.

## What I'm into right now

- Patterns for keeping AI agents *honest* — confidence thresholds, refusal modes, evaluation harnesses, structured outputs as contracts.
- Where retrieval ends and reasoning begins, and how to build interfaces that make the seam visible to users instead of hiding it.
- Cheap, durable observability for retrieval pipelines (top-K visibility, rerank-score histograms) — most "the LLM is hallucinating" complaints turn out to be retrieval problems wearing an LLM costume.

## Get in touch

- LinkedIn: *linkedin.com/in/sayandip-bagchi-3a04aa83*
- Email: *sayandip.bagchi@gmail.com*

If something in any of the repos above is useful, missing, or wrong — issues and PRs welcome.
