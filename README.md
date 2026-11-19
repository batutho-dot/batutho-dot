# Batu Thoms

I build small AI tools for sustainability and energy data, and I measure whether they are
right.

## Projects

Each repo says what it was tested on, the score it reached and where it fails.

| Project | What it shows | Result |
|---|---|---|
| [ai-toolkit](https://github.com/batutho-dot/ai-toolkit) | How I set up AI agents so their work can be checked: trust ladder, skills, worker agents, model tiers | Growing |
| [energidata-mcp](https://github.com/batutho-dot/energidata-mcp) | An MCP server that gives an AI assistant Danish power data: CO2 intensity, spot price, cleanest and cheapest hours | 10 of 10 test questions right, after one fix to my own rounding (9 of 10 before) |
| [rag-from-scratch](https://github.com/batutho-dot/rag-from-scratch) | Retrieval on EU sustainability law: word counts written by hand in numpy against a small embedding model | 6 of 10 for both at top 5, on different questions |
| [vault-mcp](https://github.com/batutho-dot/vault-mcp) | A read-only MCP server over a folder of Markdown notes that refuses every path outside it | 10 of 10 questions, 7 of 7 planted broken links found, in one run |
| Renewables and the power bill | Reproducible Python on Eurostat data | Planned |
| An evaluation set with questions that have no answer | Telling a search failure from an answer failure | Planned |

## Skills

**AI:** retrieval-augmented generation (embeddings, vector search), evaluation against
hand-checked answers, AI agents with Claude Code (skills, hooks, subagents), MCP servers,
prompt and context design

**Code and data:** Python, pandas, PostgreSQL (learning), git

## How I work with AI

1. **Small version first.** I build a toy version on invented or public data and break it
   before I touch the real thing.
2. **Numbers, not impressions.** A change is kept only if the score on the same test set
   goes up.
3. **Nothing invented.** Every value has a source that can be opened. If it is not in the
   source, the right answer is "I don't know".
4. **The agent shows what it checked.** A task ends with what was verified, what failed and
   what could not be checked.
5. **The decision stays with a person.** A model can propose a method. It does not choose
   one that changes a result.

The mechanisms behind these rules are in [ai-toolkit](https://github.com/batutho-dot/ai-toolkit).
