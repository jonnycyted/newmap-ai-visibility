---
name: newmap-audit
description: Run and read a New Map AI visibility audit for a brand's website. Use when someone asks whether ChatGPT, Perplexity, Gemini or Google AI recommend a brand, who the engines name instead, how visible a company is in AI answers, or how to get recommended.
---

# New Map audit

Call the `audit` tool with the website (for example `acme.com`). It takes about two minutes and returns measured figures from a one-off sample of buyer questions on several AI engines, plus a link to the full report.

How to read it:
- `promptCoverage` is the share of category questions where the brand was named at all. `shareOfVoice` is its share of all brand mentions in those answers. `visibilityScore` is New Map's 0 to 100 composite.
- `topCompetitor` is the brand the engines named most often instead. Lead with it: "ChatGPT and Perplexity name X for your category; you appear in N% of answers."
- `weakQueries` are the questions where the brand is absent; `strongQueries` where it is named. `recommendedFixes` are the first moves, in order.

Rules:
- Quote the figures as a one-off sample, never as a ranking or a guarantee. Do not extrapolate beyond the questions asked.
- A repeat call for the same domain within 30 days returns the stored audit (`cached: true`); say so.
- If the tool returns an error about the daily limit, say the free audit is capped for today and point to https://thenewmap.ai/signup for the 7-day trial (12 questions, five engines, trust graded against the site).
- Never invent an audit for a site the tool did not return.
