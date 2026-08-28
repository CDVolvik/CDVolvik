<div align="center">

<h1>Carlos Jimenez</h1>

<p>I build web apps, mobile apps, AI agents, and MCP servers — and run them in production.</p>

<sub>Founder @ <a href="https://www.r21digital.com/">R21 Digital</a> · Arizona + Puerto Rico · Bilingual EN/ES</sub>

</div>

---

## What I work on

- **Agent infrastructure.** A self-hosted fleet of autonomous agents, each on its own
  least-privilege identity, routed across Claude, GPT, Gemini, and Groq per task for cost and
  latency. Failed steps degrade instead of cascading.
- **MCP servers.** The tools that connect those agents to real systems — EHR data over FHIR,
  legislative records, game campaign state. Read-only by default, scoped by row-level security,
  audit-logged where the data is regulated.
- **Mobile.** A Flutter app in the field since 2025, building for six targets off one codebase.
  When a store listing is the wrong answer, I ship an installable PWA instead.
- **Full-stack product.** Next.js + Supabase + Vercel on the web, Make.com / n8n for automation,
  AWS where the compliance story requires it.
- **Enterprise IT underneath.** 15+ years, including HIPAA-regulated systems run under change
  control. It shapes how I design AI: for audit and real load, not for a demo.

## Selected work

| Project | What it is |
|---|---|
| **[practice-fusion-mcp](https://github.com/CDVolvik/practice-fusion-mcp)** | FHIR-first, read-only MCP server for the Practice Fusion EHR. Audit-logged and HIPAA-conscious — every tool call is scoped and recorded. TypeScript. |
| **[pr-legislative-x402](https://github.com/CDVolvik/pr-legislative-x402)** | Pay-per-call access to structured Puerto Rico legislative data over the x402 agent-payment standard. HTTP API + MCP server. TypeScript. |
| **[ftthelper-mcp](https://github.com/CDVolvik/ftthelper-mcp)** | Connects Claude Desktop, Cursor, or Codex to [Fantasy Tabletop Helper](https://fantasytabletophelper.com) campaigns. Read-only, scoped by Postgres row-level security. Python. |
| **[hermes-agent_Video-Research-Ingest](https://github.com/CDVolvik/hermes-agent_Video-Research-Ingest)** | Local-first pipeline turning videos and URLs into markdown notes, transcripts, metadata, and frames. Free-first by design — no paid transcription in the default path. Python. |
| **[ai-engineering-stack](https://github.com/CDVolvik/ai-engineering-stack)** | The models, agent infra, RAG, voice, and app stack I actually build and ship with. Field notes, not a link dump. |

## Production work in private repos

Client and product work I own end to end. The code isn't public, but the architecture is mine and I
can walk anyone through it.

**PRLTA angler platform** — Flutter. Tournament standings, catch logging, and vessel records for
Puerto Rico Light Tackle Anglers. 154 Dart files across 17 feature modules over a shared core: a
dependency-injection container, 27 domain services, and a 12-widget component library. One codebase
builds for iOS, Android, web, macOS, Windows, and Linux. Crash reports carry a breadcrumb buffer, so
a report arrives with the path that produced it, not just a stack trace. In the field since
2025.

**[Fantasy Tabletop Helper](https://fantasytabletophelper.com)** — Next.js + Supabase. 1,128
TypeScript files with 390 test files, 116 migrations, three CI workflows. Installable as a PWA from
a hand-written 81-line service worker instead of a plugin, because the caching rules are specific to
campaign data. Its MCP server is public, above.

## Operating what I ship

41 production sites on the books, 32 of them on Vercel, the rest mid-migration. Transactional mail
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

**Languages** TypeScript · JavaScript · Python · Dart · SQL · PHP

**Web** Next.js · React · Tailwind · shadcn/ui

**Mobile** Flutter · PWA

**Data & backend** Supabase · PostgreSQL · Node.js · Laravel

**Cloud & CI** Vercel · AWS · GitHub Actions · GitLab CI

**AI & automation** Claude · OpenAI · MCP · Make.com · n8n

## Reach me

[Website](https://www.r21digital.com/) ·
[LinkedIn](https://www.linkedin.com/in/carlos-jimenez-medinilla/) ·
[X](https://x.com/CDVolvik) ·
[cjimenez@r21digital.com](mailto:cjimenez@r21digital.com)

<div align="center">
<img height="150" src="https://github-readme-stats.vercel.app/api?username=CDVolvik&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=0a0a14&title_color=E94560&icon_color=8B5CF6&text_color=9aa0b4" alt="GitHub stats" />
</div>
