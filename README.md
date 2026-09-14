# Sayandip Bagchi

I write the specs, and I build the tooling that makes the specs cheaper to get right.

Product Leader at Zeta, in Bangalore. Fourteen years across decision sciences, edtech and fintech: Mu Sigma, a founder stint at Parentof, Director of Product at Niyo, and now Zeta. IIM Indore before that. As chapter head I run four consumer programmes with a team of twelve: a sub-prime credit card in the UK, live in operations; two credit cards in the US, one of them semi-prime and in build; and a US checking account.

The tooling is mostly retrieval systems, agents and operator tooling, so the team ships work that would normally need a bigger one. Four of the agents I have built run inside my own team:

- [derives a card programme's real stage ladder from live data, then builds the dashboard suite on top](https://github.com/SayandipBagchi/superset-bi-agent)
- [codes voice-of-customer themes from contact-centre transcripts](https://github.com/SayandipBagchi/cx-running-sheet)
- lets a PM ship copy and config changes to a programme's web app without an engineering ticket, and escalates what genuinely needs one
- answers questions over product documentation

All four derive the contract from the data, hold a strict output schema, and put a human gate in front of anything that writes. 

## Worth opening

**Code** means clone it and run it. **Write-up** means an engineering account of a system that runs on internal or client data, where the architecture and the failure modes are public and the corpus and deployment are not. **Notes** means a position rather than a system. Every write-up says so at the top.

- [superset-bi-agent](https://github.com/SayandipBagchi/superset-bi-agent) · **Code.** Builds and QCs Superset dashboard suites for card programmes, deriving each engagement's stage ladder from a transition matrix on live data. It exists because the stage names in the PRD, the event names in the warehouse and the states the data actually moves through are three different things, and a dashboard built on the first two reconciles perfectly against the wrong definition.
- [profile-optimiser-plugin](https://github.com/SayandipBagchi/profile-optimiser-plugin) · **Code.** The humanise discipline pointed at resumes, LinkedIn profiles and READMEs: two tests per line, no invented numbers, and an output gate so the rewrite does not read as generated.
- [humanise-plugin](https://github.com/SayandipBagchi/humanise-plugin) · **Code.** A Claude Code plugin that rewrites AI-shaped prose back into the writer's voice with every fact, number and citation intact, working from a catalogue of 21 named patterns. It exists because the tells are easy to name and hard to see in your own draft.
- [cx-running-sheet](https://github.com/SayandipBagchi/cx-running-sheet) · **Code.** Weekly contact-centre insights from Amazon Connect: segments separated from conversations, themes coded from transcripts only, and unique-user figures withheld when identity coverage cannot support them. Written after a single-call pull returned the first 300 rows of a much larger window and nothing looked wrong.
- [prd-builder](https://github.com/SayandipBagchi/prd-builder) · **Code.** A product requirement from source ticket through PRD, review, delivery tickets and test design, with a definition-of-ready gate the downstream skills obey. It exists because the expensive failure is not slow writing, it is a document that reads as finished and is not.
- [spa-automation-toolkit](https://github.com/SayandipBagchi/spa-automation-toolkit) · **Code.** Browser-side utilities for when the API accepts what you need and the UI will not let you do it. Zero dependencies, 22 tests, every pattern in it there because something simpler failed first.
- [amazon-connect-flow-tools](https://github.com/SayandipBagchi/amazon-connect-flow-tools) · **Code.** Renders an Amazon Connect contact flow as a draw.io diagram, and repairs and validates an export before you import it. Python stdlib only, 35 tests. Written after a failed import at 11pm before a go-live, caused by one placeholder ARN.
- [uk-compliance-knowledge-base](https://github.com/SayandipBagchi/uk-compliance-knowledge-base) · **Write-up.** Retrieval over the UK retail financial-services rulebook, 887 source documents and 16,829 chunks, with page-precise PDF citations and a rule that makes the system decline rather than paraphrase.
- [building-with-ai](https://github.com/SayandipBagchi/building-with-ai) · **Notes.** Eleven things I keep relearning about shipping retrieval systems and agents, including why the output schema is the product and what LLM-as-judge does and does not hold up for.

Also here: [enterprise-rag-knowledge-base](https://github.com/SayandipBagchi/enterprise-rag-knowledge-base) and [uat-jira-automation](https://github.com/SayandipBagchi/uat-jira-automation), both write-ups, and [geoask-prototype](https://github.com/SayandipBagchi/geoask-prototype), a product-definition package with a clickable prototype.

## Elsewhere

LinkedIn: [linkedin.com/in/sayandip-bagchi-3a04aa83](https://www.linkedin.com/in/sayandip-bagchi-3a04aa83) · Email: [sayandip.bagchi@gmail.com](mailto:sayandip.bagchi@gmail.com)

If something here is useful, missing or wrong, issues and pull requests are welcome. The write-ups especially: if you have built the same thing and reached a different conclusion, I would like to hear it.
