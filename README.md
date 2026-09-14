# Sayandip Bagchi

**Associate Director of Product @ Zeta.** Thirteen years in product across fintech,
edtech and decision sciences. I run two consumer credit card programmes — a UK
sub-prime card, live and in operations, and a US semi-prime card in build — and a
team of six.

The repositories here are the other half of that job: the retrieval systems,
agents and operator tooling I build so that a product team of six can work like a
larger one. I write the specs, and I build the things that make the specs cheaper
to get right.

---

## How to read this profile

Two kinds of repository, labelled so you do not waste a click:

- **Code** — clone it, run the tests, use it. `humanise-plugin`,
  `spa-automation-toolkit`, `amazon-connect-flow-tools`, `geoask-prototype`.
- **Write-up** — an engineering account of a system that runs on internal or
  client data and cannot be published. The architecture and the failure modes are
  here; the corpus and the deployment are not. Each one says so at the top.

I would rather label the difference than let you find it.

---

## Selected work

| Repository | Type | What it is |
|---|---|---|
| [humanise-plugin](https://github.com/sayandip1987/humanise-plugin) | Code | A Claude Code plugin: two skills, four commands, 11 eval cases, a structural validator. Rewrites AI-shaped prose back into the writer's voice with every fact, number and citation preserved, and turns a position into lines you can say out loud in a meeting. Built on a catalogue of 21 named patterns across five families. |
| [spa-automation-toolkit](https://github.com/sayandip1987/spa-automation-toolkit) | Code | Browser-side utilities for automating React SPAs when the UI blocks what the API allows: fetch interception, React Fiber traversal, `pushState` navigation that dodges unload prompts, pointer-sequence clicks for non-semantic components. Zero dependencies, 22 tests. |
| [amazon-connect-flow-tools](https://github.com/sayandip1987/amazon-connect-flow-tools) | Code | Renders an Amazon Connect contact flow as a draw.io diagram, and repairs, substitutes and validates an export before you import it. Python stdlib only — no credentials, no network. 35 tests, sanitised 31-action IVR fixture. |
| [uk-compliance-knowledge-base](https://github.com/sayandip1987/uk-compliance-knowledge-base) | Write-up | Retrieval over the UK retail financial-services rulebook — FCA Handbook, CCA 1974, PSR 2017, JMLSG, BIS. 887 source documents, 16,829 chunks, page-precise PDF citations, and a cite-or-refuse rule that makes the system decline rather than paraphrase. |
| [enterprise-rag-knowledge-base](https://github.com/sayandip1987/enterprise-rag-knowledge-base) | Write-up | Production RAG over ~2,400 chunks of internal product documentation. Intent-routed retrieval, reranking, structure-aware chunking. 4.96/5.00 on a 19-test eval; 100% in-module precision after reranking. |
| [uat-jira-automation](https://github.com/sayandip1987/uat-jira-automation) | Write-up | Agent-assisted UAT triage: dedupe against the existing board *before* filing anything. One cycle took 29 raw findings to 18 matched, 11 new and 1 comment-only, with a human gate before any write. |
| [geoask-prototype](https://github.com/sayandip1987/geoask-prototype) | Code | A product-definition package for an AI-first guidance app: strategy memo, UX spec, brand book, and a single-file clickable prototype that needs no build step. |

## Agents I've built for my own team

Less visible than the repos, and closer to the actual job. Each one exists because
a recurring analysis was eating a person's week.

- **A BI agent for card programmes.** Derives each programme's real stage ladder
  and event contract from live data — event streams, ledger, switch and auth
  tables, vendor analytics — instead of assuming it, then builds a top-down
  dashboard suite: headline, funnels, where it breaks, why. Every number
  triangulated across at least two sources, with QC gates and a definition
  registry that records the caveats. It also turns event counts into
  affected-population views, which is the question people actually mean when they
  ask about declines.
- **A contact-centre insights agent.** Pulls chat and call data, codes
  voice-of-customer themes from transcripts, computes queue funnel and handle-time
  metrics, and publishes a running sheet that refreshes on a schedule with
  period-over-period deltas.
- **A front-end change agent.** Lets a PM ship copy and config changes to a card
  programme's web app without an engineering ticket — and hard-escalates anything
  that genuinely needs one. Triage, execute, verify, ship, with blocking QC gates
  and an explicit deploy handoff. The escalation boundary is the point of it.
- **An internal knowledge base.** RAG over product documentation for a company
  where the answer usually exists and nobody can find it.

The pattern across all four: derive the contract from the data rather than
assuming it, make the output schema strict, and put a human gate in front of
anything that writes.

## How I think about building with AI

- **Boring before clever.** Better chunking and a reranker beat HyDE and graph
  indexes on most corpora. Coordinate clicks beat clever DOM heuristics on
  Atlaskit. Reach for the sophisticated thing after the boring thing has hit a
  measured ceiling, not before.
- **The schema of the output is the product.** "Tell me what's broken" produces
  unreviewable noise. A strict findings packet — citation, repro, evidence,
  confidence — produces a queue people respect and act on.
- **The eval harness is architecture, not QA.** It is the thing that lets you move
  retrieval quality in one direction instead of trading one regression for
  another. Build it before you need it.
- **Run inside the user's session.** Re-implementing SSO and MFA in a headless
  harness is almost always a worse use of time than borrowing a logged-in browser
  and being deliberate about side effects.
- **Reversibility is a feature.** Backups before destructive ingest.
  Validate-before-promote. Dry runs that print the diff. Every project here has a
  "we can roll this back" story built in, because the ones that did not taught me
  to.
- **Most hallucination complaints are retrieval problems wearing a costume.**
  Cheap observability on the retrieval step — top-K visibility, rerank-score
  histograms — resolves more of them than prompt engineering does.

## What I'm working on now

- Keeping agents honest: confidence thresholds, refusal modes, structured outputs
  as contracts, and evals that catch drift rather than describe it after the fact.
- Where retrieval ends and reasoning begins, and interfaces that show the reader
  that seam instead of hiding it.
- Compliance-aware retrieval — systems that decline to answer when the rulebook
  does not say, which turns out to be the hard half.

## Elsewhere

- LinkedIn — [linkedin.com/in/sayandip-bagchi-3a04aa83](https://www.linkedin.com/in/sayandip-bagchi-3a04aa83)
- Email — [sayandip.bagchi@gmail.com](mailto:sayandip.bagchi@gmail.com)
- Based in Bangalore, India

If something in any repository here is useful, missing, or wrong, issues and pull
requests are welcome. The write-ups especially: if you have built the same thing
and reached a different conclusion, I would like to hear it.
