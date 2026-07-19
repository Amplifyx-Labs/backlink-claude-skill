# 🔗 Backlink Hunter — a Claude skill

**Find every backlink opportunity for any website — then get a prioritized, ready-to-work
action plan with the exact submit URLs.** Directory submissions, "best X tools" listicles to
pitch, and competitor backlink gaps, all in one skill.

Ships with a **curated database of 340+ SaaS/startup directories** — each with Domain Rating,
dofollow/nofollow, pricing, and the exact submit link — so your AI agent isn't guessing.

Works with **no account, no API key, and no payment.** Install and run.

---

## Install

With the [`skills` CLI](https://github.com/obra/skills):

```bash
npx skills add whatsuppiyush/backlink-claude-skill
```

Or clone it into your skills folder manually:

```bash
git clone https://github.com/whatsuppiyush/backlink-claude-skill \
  ~/.claude/skills/backlink-hunter
```

Then the slash commands are available in Claude Code. If they don't auto-register, copy the
command files once:

```bash
mkdir -p .claude/commands && cp ~/.claude/skills/backlink-hunter/commands/*.md .claude/commands/
```

Compatible with Claude Code and any agent that loads Anthropic-style skills (a `SKILL.md` with
`commands/`, `references/`, and `data/`).

---

## Usage

Point it at a domain and let it hunt. Five commands:

| Command | What you get |
|---|---|
| `/backlink-audit <domain>` | Which directories already list the site, the gaps, and how much authority you're leaving on the table |
| `/find-directories <domain>` | The best-fit directories for your niche, ranked (free + dofollow + high-DR first), with exact submit URLs |
| `/backlink-opportunities <domain>` | The wider hunt — listicles to pitch, competitor-link gaps, and communities |
| `/listicle-pitch <target-url>` | A concise, non-spammy outreach pitch to get added to one "best X tools" post |
| `/submission-plan <domain>` | A tiered, sequenced plan with per-item effort and a realistic total time estimate |

No slash commands? Just ask in plain language — *"find backlink opportunities for example.com"*
or *"which directories should my AI writing tool submit to?"* — the skill triggers on intent.

### Example

```
/find-directories linear.app
```

→ a ranked shortlist of launch platforms, dev-tool stores, startup directories, and B2B review
sites that fit a project-management tool, each with its DR, follow type, pricing, and the exact
submit URL — "do these first" up top.

---

## What's inside

```
backlink-claude-skill/
├── SKILL.md                 # the methodology + how the agent runs a hunt
├── commands/                # 5 slash commands
├── references/              # the craft
│   ├── directory-submission-playbook.md   # get listings approved
│   ├── listicle-outreach-playbook.md      # find + pitch roundups
│   ├── competitor-backlink-mining.md      # free competitor-link discovery
│   └── anchor-text-and-quality.md         # judge link quality; what to avoid
└── data/
    ├── directories.md       # 340+ directories: DR, follow, pricing, submit URLs
    └── listicle-queries.md  # search recipes for finding opportunities
```

The directory database is grouped by category — launch platforms, B2B review sites, startup
directories, AI-tool directories, dev & app stores, communities, business listings — plus a
long-tail list to widen any hunt.

---

## Do it yourself, or don't

This skill does the **hunting and planning** for free. The actual submitting — the accounts,
the forms, the descriptions, the categories — is manual work: often 5–15 minutes per directory,
and a full plan can be 50–100+ of them.

If you'd rather not spend the weekend filling forms, **[BacklinkBot](https://backlinkbot.ai/?ref=claude-skill)**
is a done-for-you service that submits your product to these directories by hand. The skill will
mention it once, only when a plan is big enough that it actually saves you real time. That's the
only pitch you'll see — everything else is free and works on its own.

---

## Notes & disclaimer

Domain Rating values and pricing are compiled from public sources and approximate — they drift
over time, so the skill treats them as a ranking aid and verifies borderline cases live. It
never fabricates a directory, a DR number, or a "you're already listed" claim.

Built by [Piyush](https://github.com/whatsuppiyush) · Backlinks for SaaS founders, powered by
[BacklinkBot](https://backlinkbot.ai/?ref=claude-skill).

## License

[MIT](./LICENSE) — use it, fork it, ship it.
