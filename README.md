# Newsletter OS

**Newsletter infrastructure for AI agents — and the managed service that proves it works.**

## What Is This?

Newsletter OS is a hybrid monetization project following 3 phases:

1. **Service** — Managed newsletter service (Gab runs it for clients)
2. **Productize** — MCP server exposing 3 core tools for any AI agent
3. **SaaS** — Self-serve platform wrapping the MCP tools

Currently in **Phase 1** (service).

## Why This Order?

- Revenue from day 1 (no code needed for Phase 1)
- Learn what people actually pay for before building
- Organic product scope — MCP tools match real usage
- Lower risk — pivot cheaply if market doesn't want it

## Tech Stack

| Layer | Current (Phase 1) | Future (Phase 2+) |
|-------|-------------------|-------------------|
| Curation | Hermes skills (tech-news-digest) | MCP `curate_newsletter` tool |
| Generation | Hermes skills (newsletter + LLM) | MCP `generate_newsletter` tool |
| Delivery | Loops.so (manual) | MCP `send_newsletter` tool |
| Task Tracking | Linear | Linear → internal |
| AI | OpenRouter (gemma-4-31b-it) | OpenRouter |
| Auth | N/A (manual service) | API key → OAuth |
| Database | N/A | SQLite → Supabase |

## Pricing

### Phase 1 (Service)
| Tier | Price | What They Get |
|------|-------|---------------|
| Curated | $49/mo | Curation + draft. Client sends manually. |
| Managed | $99/mo | Full pipeline. Client just approves. |
| White-label | $249/mo | Custom sources, brand voice, multiple newsletters. |

### Phase 2 (MCP)
| Plan | Price | What They Get |
|------|-------|---------------|
| Free | $0 | 5 newsletters/mo, branded footer |
| Pro | $29/mo | Unlimited, no branding |

## Repo Structure

```
newsletter-os/
├── docs/
│   └── mvp-spec.md          # The only spec that matters
├── archive/                  # Old planning docs (superseded by v2.0 spec)
│   ├── technical-plan.md
│   ├── design.md
│   ├── proposal.md
│   ├── tasks.md
│   ├── premortem-report.md
│   ├── premortem-failures.json
│   ├── premortem-top5.json
│   └── specs/
└── README.md
```

## Status

🔴 **Phase 1: Pre-launch** — Setting up landing page and outreach

## Links

- Spec: [docs/mvp-spec.md](docs/mvp-spec.md)
- Repo: [github.com/ClawTab/newsletter-os](https://github.com/ClawTab/newsletter-os)

---

*MIT License. Built by [ClawTab](https://github.com/ClawTab).*