<p align="center">
  <a href="https://anypost.md">
    <img src="static/logo.png" alt="AnyPost" width="120" />
  </a>
</p>

<h1 align="center">AnyPost</h1>

<p align="center">
  <strong>Social posts as clean Markdown — built by agents, for agents.</strong>
</p>

<p align="center">
  <a href="https://anypost.md"><img src="https://img.shields.io/badge/website-anypost.md-3d5a45?style=flat-square" alt="anypost.md" /></a>
  <a href="https://anypost.md/free-tools"><img src="https://img.shields.io/badge/free_tools-14+_guest_tools-5a7a62?style=flat-square" alt="Free tools" /></a>
  <a href="https://anypost.md/i/skill.md"><img src="https://img.shields.io/badge/agent_skill-anypost--md-7a9a82?style=flat-square" alt="Agent skill" /></a>
  <a href="https://webmachinelearning.github.io/webmcp/"><img src="https://img.shields.io/badge/WebMCP-preview-8fb89a?style=flat-square" alt="WebMCP" /></a>
</p>

<p align="center">
  <a href="#highlights">Highlights</a> ·
  <a href="#domain-swap">Domain swap</a> ·
  <a href="#free-tools">Free tools</a> ·
  <a href="#webmcp">WebMCP</a> ·
  <a href="#platforms">Platforms</a> ·
  <a href="#for-agents">For agents</a>
</p>

---

> Swap the domain on a social post URL and get LLM-ready Markdown back — no extension, no copy-paste circus, no generic page scraping.

AnyPost turns **social post links** (X, LinkedIn, Reddit, Threads, Bluesky, and more) into **clean Markdown** your agents can read, cite, and summarize. Humans get the same trick in the browser; agents get domain swap, free guest tools, and optional **WebMCP** tools when the tab is open.

- **Product:** [anypost.md](https://anypost.md)
- **Free tools hub:** [anypost.md/free-tools](https://anypost.md/free-tools)
- **Live preview:** [anypost.md/preview](https://anypost.md/preview)
- **Agent skill:** [anypost.md/i/skill.md](https://anypost.md/i/skill.md)
- **Docs:** [anypost.md/docs](https://anypost.md/docs)

---

## Highlights

- **One memorable trick** — replace `x.com` (or any supported host) with `anypost.md` and prefix the path with the platform slug.
- **Social-first** — built for posts and threads, not arbitrary homepages or docs sites.
- **Free guest tools** — Compose, post preview, GEO checker, llms.txt generator, and more run in the browser with no signup.
- **WebMCP preview** — browser agents discover `convert_post` and `list_supported_platforms` on anypost.md without DOM scraping.
- **Reverse workflow** — [Compose](https://anypost.md/compose) drafts Markdown → social posts (LinkedIn, X, Instagram, Reddit, Discord, and more).

---

## Domain swap

Three steps. No SDK required.

**01 — Open any post**  
Copy a public post or thread URL from X, Reddit, Bluesky, Threads, LinkedIn, or another supported network.

**02 — Swap the domain**  
Change the host to `anypost.md` and keep the path — add the platform slug when the host alone is not enough.

**03 — Read Markdown**  
The response is plain, LLM-ready Markdown: author, body, media, stats, and a source link.

### Examples

```text
https://x.com/jack/status/20
→ https://anypost.md/x/jack/status/20

https://www.reddit.com/r/python/comments/abc123/title_slug/
→ https://anypost.md/reddit/r/python/comments/abc123/title_slug/

https://bsky.app/profile/user.bsky.social/post/3jz7abc
→ https://anypost.md/bluesky/profile/user.bsky.social/post/3jz7abc

https://news.ycombinator.com/item?id=12345678
→ https://anypost.md/hackernews/item?id=12345678
```

Mastodon is instance-based:

```text
https://mastodon.social/@user/123456789
→ https://anypost.md/mastodon/mastodon.social/@user/123456789
```

Paste the swapped URL in a browser, `curl`, or your agent — you get readable Markdown instead of a heavy social UI.

**Try it:** [anypost.md/preview](https://anypost.md/preview) · per-platform guides at [anypost.md/convert](https://anypost.md/convert)

---

## Free tools

Guest tools at [anypost.md/free-tools](https://anypost.md/free-tools) — browser-only, no API key, no backend credits for drafting and SEO utilities.

| Tool | What it does |
|------|----------------|
| [Compose](https://anypost.md/compose) | Markdown → social posts with live preview for 12+ networks |
| [Post preview](https://anypost.md/free-tools/post-preview) | Mock X, LinkedIn, Threads, Bluesky, Instagram cards before publish |
| [Post linter](https://anypost.md/free-tools/post-linter) | Score drafts for length, hooks, hashtags, and engagement |
| [LinkedIn formatter](https://anypost.md/free-tools/linkedin-formatter) | Unicode bold/italic styles for LinkedIn posts |
| [URL to Markdown](https://anypost.md/free-tools/url-to-markdown) | Paste a social post URL → clean Markdown (free tier) |
| [llms.txt generator](https://anypost.md/free-tools/llms-txt-generator) | Build a spec-compliant `llms.txt` for your domain |
| [GEO checker](https://anypost.md/free-tools/geo-checker) | Score pages for AI answer engines and crawler access |
| [Sitemap builder](https://anypost.md/free-tools/sitemap-builder) | Generate `sitemap.xml` for Search Console / Bing WMT |
| [JSON-LD extractor](https://anypost.md/free-tools/structured-data-extractor) | Pull Schema.org blocks from a URL or HTML paste |
| [Social card checker](https://anypost.md/free-tools/social-card-checker) | Validate Open Graph / Twitter Card tags |
| [DESIGN.md generator](https://anypost.md/free-tools/design-md-generator) | Export UI tokens for AI coding agents |
| [Font finder](https://anypost.md/free-tools/font-finder) | Detect `font-family` stacks on public pages |
| [Live preview](https://anypost.md/preview) | Real-time convert demo + WebMCP registration |
| [Save tokens](https://anypost.md/save-tokens) | Why clean post Markdown beats raw HTML for LLMs |

---

## WebMCP

[WebMCP](https://webmachinelearning.github.io/webmcp/) lets capable browsers expose **structured tools** to on-page AI agents. AnyPost registers tools on every page so agents can convert posts without scraping the DOM.

| Tool | Purpose |
|------|---------|
| `convert_post` | Pass a social post `url` → receive clean Markdown (same pipeline as domain swap) |
| `list_supported_platforms` | List live platforms, free-tier flags, and HTTP fallbacks when WebMCP is off |

**Enable (preview):** Chrome 146+ Canary → `chrome://flags` → enable **WebMCP** → reload [anypost.md](https://anypost.md).

**Headless agents:** keep using **domain swap** or install the [anypost-md agent skill](https://anypost.md/i/skill.md). WebMCP is for human-driven browser sessions today.

Docs: [anypost.md/docs#webmcp](https://anypost.md/docs#webmcp)

---

## Platforms

Live sources include **X**, **Reddit**, **Bluesky**, **Mastodon**, **Hacker News**, **YouTube**, **Substack**, **Threads**, **LinkedIn**, **Instagram**, **Facebook**, **Pinterest**, **TikTok**, and **Medium**.

Per-platform landing pages and agent guides: [anypost.md/convert](https://anypost.md/convert) · [anypost.md/guides](https://anypost.md/guides)

---

## For agents

Install the public skill (no clone required):

```text
https://anypost.md/i/skill.md
```

Cursor / Claude Code: add `.cursor/skills/anypost-md/SKILL.md` or fetch the URL above. The skill teaches agents when to swap domains, which free tools to use for drafting, and how WebMCP fits alongside HTTP.

**Human login:** [anypost.md/login](https://anypost.md/login)  
**Pricing (credits):** [anypost.md/pricing](https://anypost.md/pricing)

---

## About this repo

This organization hosts **AnyPost** open assets — agent skills, docs mirrors, and community examples around [anypost.md](https://anypost.md).

The production app lives in private deployment; this README is the public face of the project on GitHub.

---

<p align="center">
  <a href="https://anypost.md">anypost.md</a> ·
  <a href="https://anypost.md/free-tools">Free tools</a> ·
  <a href="https://anypost.md/docs">Docs</a> ·
  <a href="https://anypost.md/contact">Contact</a>
</p>

<p align="center">
  <sub>Built by agents, for agents.</sub>
</p>
