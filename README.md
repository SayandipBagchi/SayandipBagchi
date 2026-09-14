# Sayandip Bagchi

I write the specs, and I build the tooling that makes the specs cheaper to get right.

Product Leader at Zeta, in Bangalore. Fourteen years across decision sciences, edtech and fintech: Mu Sigma, a founder stint at Parentof, Director of Product at Niyo, and now Zeta. IIM Indore before that. As chapter head I run four consumer programmes with a team of twelve: a sub-prime credit card in the UK, live in operations; two credit cards in the US, one of them semi-prime and in build; and a US checking account.

The tooling is mostly retrieval systems, agents and operator tooling, so the team ships work that would normally need a bigger one. Four of the agents I have built run inside my own team:

- derives a card programme's real stage ladder from live data, then builds the dashboard suite on top
- codes voice-of-customer themes from contact-centre transcripts
- lets a PM ship copy and config changes to a programme's web app without an engineering ticket, and escalates what genuinely needs one
- answers questions over product documentation

All four derive the contract from the data, hold a strict output schema, and put a human gate in front of anything that writes.

## Worth opening

**Code** means clone it and run it. **Write-up** means an engineering account of a system that runs on internal or client data, where the architecture and the failure modes are public and the corpus and deployment are not. **Notes** means a position rather than a system. Every write-up says so at the top.

- [humanise-plugin](https://github.com/sayandip1987/humanise-plugin) · **Code.** A Claude Code plugin that rewrites AI-shaped prose back into the writer's voice with every fact, number and citation intact, working from a catalogue of 21 named patterns. It exists because the tells are easy to name and hard to see in your own draft.
- [profile-optimiser-plugin](https://github.com/sayandip1987/profile-optimiser-plugin) · **Code.** The same discipline pointed at resumes, LinkedIn profiles and READMEs: two tests per line, no invented numbers, and an output gate so the rewrite does not read as generated.
- [spa-automation-toolkit](https://github.com/sayandip1987/spa-automation-toolkit) · **Code.** Browser-side utilities for when the API accepts what you need and the UI will not let you do it. Zero dependencies, 22 tests, every pattern in it there because something simpler failed first.
- [amazon-connect-flow-tools](https://github.com/sayandip1987/amazon-connect-flow-tools) · **Code.** Renders an Amazon Connect contact flow as a draw.io diagram, and repairs and validates an export before you import it. Python stdlib only, 35 tests. Written after a failed import at 11pm before a go-live, caused by one placeholder ARN.
- [uk-compliance-knowledge-base](https://github.com/sayandip1987/uk-compliance-knowledge-base) · **Write-up.** Retrieval over the UK retail financial-services rulebook, 887 source documents and 16,829 chunks, with page-precise PDF citations and a rule that makes the system decline rather than paraphrase.
- [building-with-ai](https://github.com/sayandip1987/building-with-ai) · **Notes.** Eleven things I keep relearning about shipping retrieval systems and agents, including why the output schema is the product and what LLM-as-judge does and does not hold up for.

Also here: [enterprise-rag-knowledge-base](https://github.com/sayandip1987/enterprise-rag-knowledge-base) and [uat-jira-automation](https://github.com/sayandip1987/uat-jira-automation), both write-ups, and [geoask-prototype](https://github.com/sayandip1987/geoask-prototype), a product-definition package with a clickable prototype.

## Elsewhere

LinkedIn: [linkedin.com/in/sayandip-bagchi-3a04aa83](https://www.linkedin.com/in/sayandip-bagchi-3a04aa83) · Email: [sayandip.bagchi@gmail.com](mailto:sayandip.bagchi@gmail.com)

If something here is useful, missing or wrong, issues and pull requests are welcome. The write-ups especially: if you have built the same thing and reached a different conclusion, I would like to hear it.
