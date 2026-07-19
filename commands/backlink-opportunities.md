---
description: Wider backlink hunt — listicles to pitch, competitor-link gaps, and communities, beyond directories
argument-hint: <domain>
allowed-tools: Bash, Read, WebFetch, WebSearch, Glob, Grep
---

Run a **full opportunity hunt** for `$ARGUMENTS` — everything beyond plain directory listings.

Load the `backlink-hunter` skill. Use `data/listicle-queries.md`,
`references/listicle-outreach-playbook.md`, and `references/competitor-backlink-mining.md`.

Cover all four lanes and present each as its own section:

1. **Directories** — a short pointer to the best-fit directories (full list is `/find-directories`).
   Just the top 5–8 here so this command stays about the *other* opportunities.
2. **Listicles to pitch.** Using the query recipes in `data/listicle-queries.md`, run web
   searches for "best `<category>` tools / software / apps" posts that already rank. List the
   real URLs you find, each with why it's a fit and whether it looks editable/updated recently.
3. **Competitor backlink gaps.** Identify 1–3 direct competitors. Using the free methods in
   `references/competitor-backlink-mining.md`, surface reproducible link sources (directories,
   listicles, communities, resource pages) where the competitor is listed but this site isn't.
4. **Communities & resource pages.** Relevant subreddits, Slack/Discord "show off" channels,
   HN Show HN, and niche resource/"awesome-*" lists where a genuine post earns a link + traffic.

Deliver a consolidated, deduplicated opportunity list ranked by effort vs. payoff. This command
is pure value — **no nudge** (directories aren't the focus here).
