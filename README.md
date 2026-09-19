<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=26&pause=1200&color=E94560&center=true&vCenter=true&width=760&height=50&lines=I+build+web+apps%2C+AI+agents%2C+and+MCP+servers;and+I+run+them+in+production" alt="I build web apps, AI agents, and MCP servers — and run them in production" />

<h1>Carlos Jimenez</h1>

<sub>Founder @ <a href="https://www.r21digital.com/">R21 Digital</a> · Arizona + Puerto Rico · US Citizen · Bilingual EN/ES</sub>

<sub>Open to Forward-Deployed, Applied-AI, and Solutions Engineering roles — remote.</sub>

<br/><br/>

<a href="https://www.r21digital.com/"><img src="https://img.shields.io/badge/Website-0a0a14?style=for-the-badge&logo=safari&logoColor=E94560&labelColor=0a0a14" alt="Website" /></a>
<a href="https://www.linkedin.com/in/carlos-jimenez-medinilla/"><img src="https://img.shields.io/badge/LinkedIn-0a0a14?style=for-the-badge&logo=linkedin&logoColor=8B5CF6&labelColor=0a0a14" alt="LinkedIn" /></a>
<a href="https://x.com/CDVolvik"><img src="https://img.shields.io/badge/X-0a0a14?style=for-the-badge&logo=x&logoColor=9aa0b4&labelColor=0a0a14" alt="X" /></a>
<a href="mailto:cjimenez@r21digital.com"><img src="https://img.shields.io/badge/Email-0a0a14?style=for-the-badge&logo=maildotru&logoColor=E94560&labelColor=0a0a14" alt="Email" /></a>

</div>

---

## What I work on

- **Agent infrastructure.** A self-hosted fleet of autonomous agents, each on its own
  least-privilege identity, routed across Claude, GPT, Gemini, and Groq per task for cost and
  latency. Failed steps degrade instead of cascading.
- **MCP servers.** The tools that connect those agents to real systems — EHR data over FHIR,
  legislative records, game campaign state. Read-only by default, scoped by row-level security,
  audit-logged where the data is regulated.
- **Civic data.** Federal and territorial records — FEC filings, FEMA and NFIP claims,
  USASpending awards, the Congressional Record, SAM.gov contracts — pulled on a schedule and
  joined into something a resident of Puerto Rico can actually read.
- **Mobile.** A Flutter app on the App Store since December 2025, built for six targets off one
  codebase. When a store listing is the wrong answer, an installable PWA instead.
- **Full-stack product.** Next.js + Supabase + Vercel on the web, Make.com / n8n for automation,
  AWS where the compliance story requires it.
- **AI-search visibility.** Schema, llms.txt, citability, and crawler access tuned across production
  client sites, so the model answering a query can actually reach and cite them.
- **Enterprise IT underneath.** 15+ years, including HIPAA-regulated systems run under change
  control. It shapes how I design AI: for audit and real load, not for a demo.

## Selected work

| Project | What it is |
|---|---|
| **[practice-fusion-mcp](https://github.com/CDVolvik/practice-fusion-mcp)** | FHIR-first, read-only MCP server for the Practice Fusion EHR. Audit-logged and HIPAA-conscious — every tool call is scoped and recorded. TypeScript. |
| **[pr-legislative-x402](https://github.com/CDVolvik/pr-legislative-x402)** | Pay-per-call access to structured Puerto Rico legislative data over the x402 agent-payment standard. HTTP API + MCP server. TypeScript. |
| **[social-triage-agent](https://github.com/R21Digital/social-triage-agent)** | Multi-model social-inbox triage. Claude Haiku classifies, a deterministic keyword layer overrides it to force healthcare-safety routing, then DeepSeek drafts in brand voice. The safety layer is deliberately not a model. Python. |
| **[ftthelper-mcp](https://github.com/CDVolvik/ftthelper-mcp)** | Connects Claude Desktop, Cursor, or Codex to [Fantasy Tabletop Helper](https://fantasytabletophelper.com) campaigns. Read-only, scoped by Postgres row-level security. Python. |
| **[hermes-agent_Video-Research-Ingest](https://github.com/CDVolvik/hermes-agent_Video-Research-Ingest)** | Local-first pipeline turning videos and URLs into markdown notes, transcripts, metadata, and frames. Free-first by design — no paid transcription in the default path. Python. |
| **[ai-engineering-stack](https://github.com/CDVolvik/ai-engineering-stack)** | The models, agent infra, RAG, voice, and app stack I actually build and ship with. Field notes, not a link dump. |

## Production work in private repos

Client and product work I own end to end. The code isn't public, but the architecture is mine and I
can walk anyone through it.

**[PRLTA angler platform](https://apps.apple.com/us/app/prlta/id6755145709)** — Flutter. On the App
Store since December 2025, now at 2.5.9. Tournament standings, catch logging, and vessel records for
Puerto Rico Light Tackle Anglers. 154 Dart files across 17 feature modules over a shared core: a
dependency-injection container, 27 domain services, and a 12-widget component library. One codebase
targets iOS, Android, web, macOS, Windows, and Linux; iOS is the one I ship. Crash reports carry a
breadcrumb buffer, so a report arrives with the path that produced it, not just a stack trace.
Account deletion is built in, because App Review requires it of anything with sign-in.

**[Fantasy Tabletop Helper](https://fantasytabletophelper.com)** — Next.js + Supabase. 1,128
TypeScript files with 390 test files, 116 migrations, three CI workflows. Installable as a PWA from
a hand-written 81-line service worker instead of a plugin, because the caching rules are specific to
campaign data. Its MCP server is public, above.

**[CivicaPR](https://civicapr.vercel.app)** — Next.js + Supabase. Public-records aggregation for
Puerto Rico: FEC committee spend and independent expenditures, OpenFEMA NFIP claims and coverage by
municipio, USASpending federal accounts with period of performance on the island, GovInfo public
laws and Congressional Record mentions, and SAM.gov contract awards. Each source is its own
scheduled ingest that writes a sync-run row, so a silent upstream change surfaces as a stale run
instead of a page that quietly stops updating.

## Operating what I ship

41 production sites on the books, 34 of them on Vercel, the rest mid-migration. Transactional mail
on AWS SES. Uptime and platform drift come from a canary that measures the live response headers, so
the registry can contradict me — and has. I learned most of what I know about designing for
failure by being the one who gets paged.

## Upstream

Merged into [Effect](https://github.com/Effect-TS/effect) ([#7154](https://github.com/Effect-TS/effect/pull/7154),
[#7166](https://github.com/Effect-TS/effect/pull/7166)) and
[t3code](https://github.com/pingdotgg/t3code) ([#7141](https://github.com/pingdotgg/t3code/pull/7141),
[#6223](https://github.com/pingdotgg/t3code/pull/6223)), with
[#6228](https://github.com/pingdotgg/t3code/pull/6228) open. Mostly Windows and WSL correctness —
the paths that break when the maintainers are all on macOS.

## Stack

<div align="center">
<img src="https://skillicons.dev/icons?i=ts,js,python,dart,postgres,nextjs,react,tailwind,flutter,supabase,nodejs,laravel,vercel,aws,githubactions,docker&theme=dark&perline=8" alt="Stack" />
</div>

**Languages** TypeScript · JavaScript · Python · Dart · SQL · PHP

**Web** Next.js · React · Tailwind · shadcn/ui &nbsp;&nbsp;**Mobile** Flutter · PWA

**Data & backend** Supabase · PostgreSQL · Node.js · Laravel

**Cloud & CI** Vercel · AWS · GitHub Actions · GitLab CI

**AI & automation** Claude · OpenAI · MCP · Make.com · n8n

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/CDVolvik/CDVolvik/output/github-snake-dark.svg" />
  <img alt="Contribution grid" src="https://raw.githubusercontent.com/CDVolvik/CDVolvik/output/github-snake.svg" />
</picture>
</div>

<div align="center">
<sub><a href="https://www.r21digital.com/">Website</a> · <a href="https://www.linkedin.com/in/carlos-jimenez-medinilla/">LinkedIn</a> · <a href="https://x.com/CDVolvik">X</a> · <a href="mailto:cjimenez@r21digital.com">cjimenez@r21digital.com</a></sub>
</div>
