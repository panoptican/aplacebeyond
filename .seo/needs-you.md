# Needs you

Decisions, logins, reviews, and keys only a human can provide. The skill writes the `question` column. You write the `answer` column. The next run acts on any row with an answer and no `closed` date, then stamps it.

Keep answers to one line where you can. If the answer is "never" or "not now," say that; the row closes and the blocked candidate is dropped or deferred.

| id | opened | blocks | question | answer | closed |
|---|---|---|---|---|---|
| NY-1 | 2026-09-11 | all measurement (GSC panels, census verdicts, priors) | Connect Google Search Console: verify https://aplacebeyond.place as a domain property, then give this host a Search Console client (an MCP server authenticated with a Google account that has at least Full access). Say "skip Search Console" to stop seeing this. | done — verified/connected by user | 2026-09-11 |
| NY-2 | 2026-09-11 | nothing (confirmed by interview, 2026-09-11) | Confirm the positioning sentence in `.seo/brand.md`: "The audio accompaniment to the book *A Place Beyond* by Garett Strickland — ambient music and visuals for reading." Edit `.seo/brand.md` if anything is off. | confirmed in interview | 2026-09-11 |
| NY-3 | 2026-09-11 | Phase 1 (stating the book relationship on-page) | The homepage says nothing about the book, the author, or the composer. Should I rewrite the on-page copy + metadata to state the relationship (title/meta mention the book, composer credit for Garett Strickland, link out to the Asterism product page)? Options: (a) yes, do it this run; (b) later, keep Phase 1 pending; (c) never — the site stays deliberately wordless. | later, keep Phase 1 pending | 2026-09-11 |
| NY-4 | 2026-09-11 | offpage brief (Phase 2) | Who can edit the Asterism Books product listing or publisher site to add a link to aplacebeyond.place — you, or do we ask Inside the Castle/Asterism? (We only write the brief; a human sends it.) | nobody can — drop offpage brief | 2026-09-11 |
| NY-5 | 2026-09-11 | answer-engine presence (robots.txt posture) | The live robots.txt serves Cloudflare Managed Content that disallows GPTBot, ClaudeBot, Google-Extended, CCBot, Bytespider, Applebot-Extended, meta-externalagent and Amazonbot (ai-train=no, use=reference). ChatGPT/Claude/Gemini cannot fetch or cite the site today. Should I re-allow the citing crawlers in robots.txt (keep ai-train=no)? (a) allow all AI crawlers to read/cite; (b) keep everything blocked; (c) allow citing bots but keep training bots off (same as (a) in practice today). | allow citing bots, keep training reserved — answered "Both" at the 2026-09-11 checkpoint; robots.txt edited that run | 2026-09-11 |
| NY-6 | 2026-09-11 | AEO attribution | AI referral attribution is not measured: no GA4 connected and no access logs configured. Connect GA4 or point me at the host's access logs if you want "AI referrals" measured instead of guessed. | uses Umami — script installed in index.html this session | 2026-09-11 |

<!-- All rows closed 2026-09-11. NY-4 dropped: nobody can edit the Asterism/publisher pages → offpage brief dropped. NY-6: user uses Umami, script installed in index.html. -->
