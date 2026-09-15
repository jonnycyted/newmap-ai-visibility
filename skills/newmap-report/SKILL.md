---
name: newmap-report
description: Read a New Map client's live AI visibility data (weekly measurement on seven engines) and answer questions about trust, discovery, competitors, prompts and citations. Use when a signed-in New Map client asks how they are doing in AI answers this week, what changed, who is named instead of them, or which sources the engines cite.
---

# New Map client data

These tools need a client key (see SETUP.md). They are read-only and scoped to the client's workspace:
- `geo_read`: the latest weekly reading (trust and visibility on their own denominators).
- `trend_read`: week-over-week movement. Only claim movement when the feed has advanced.
- `answers_read`: the verbatim engine answers for a prompt.
- `prompts_read`: the tracked questions and how each performs.
- `competitor_read`: who is named instead, by engine and position.
- `citations_read`: the domains and URLs the engines cite for the category.

Rules:
- Two KPIs, never blended: trust (branded answers accurate, current, evidenced) and visibility (named on category questions).
- Every number comes from a tool result in this conversation. Quote it with its date. No estimates.
- When asked "what should we do", ground it in the data: name the prompts lost, the rival named, the sources cited, then the fix (site correction, Answer Library page, placement).
