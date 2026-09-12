# A Place Beyond — Content Ledger

> The memory of the engine. Read first on every `/seo` run: the **Shipped** table is the dedup record (never re-write a covered topic); the **Performance** table is the scoreboard (did the last pieces actually work?); the **Candidate backlog** is the scored shortlist so each run starts warm. Updated in the same edit batch as every piece shipped.

---

## Shipped

| Date | Title | Type | Slug / URL | Target keyword | Vol | Bucket | Original data (source · n · as-of) | Refresh due | Primary internal links | Commit / PR |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 2026-02-18 | A Place Beyond (homepage) | resource | `/` | A Place Beyond | — | easy | none | n/a | — | 17cf9a4 |
| 2026-09-11 | repair: homepage h1 | repair | `/` | — | — | — | health_diff 2026-09-12: h1_count=0 → added visually-hidden h1 | n/a | — | uncommitted |
| 2026-09-11 | repair: robots.txt AI-crawler access | repair | /robots.txt | — | — | — | live robots.txt (Cloudflare Managed Content) disallowed GPTBot/ClaudeBot/Google-Extended/CCBot/Bytespider/Applebot-Extended/meta-externalagent/Amazonbot → re-allowed 16 answer-engine crawlers; ai-train stays reserved | n/a | — | uncommitted |
| 2026-09-11 | instrumentation: Umami analytics script | tool | `/` | — | — | — | NY-6: user uses Umami (self-hosted, analytics.spidleweb.net); defer script + site id added to index.html head | n/a | — | uncommitted |

<!-- Append one row per piece at Step 5. Type ∈ guide | how-to | listicle | definition | comparison | data-study | resource | opinion | case-study | tool -->

---

## Performance

> The closed loop. Filled by **Step 0.5** of a later run from GSC (`references/gsc.md` §2), seeded as `unmeasured` when a piece ships.

> **Backfilled:** never — GSC not connected as of 2026-09-11. Until it is, no piece can be measured; the homepage row stays `unmeasured`.

| Slug / URL | Published | Indexed? (state · checked) | Read @28d (clicks · impr · pos) | Read @56d (clicks · impr · pos) | Site-wide same window (clicks · impr) | Best lever (recover/CTR/rank · est. clicks) | State | Note / next action |
|---|---|---|---|---|---|---|---|---|---|
| `/` | 2026-02-18 | unknown · never | — | — | — | — | unmeasured | Index status unknown until GSC is connected or a `site:` check is run |

---

## Candidate backlog

> Scored shortlist from the last selection run. The next run reads this before regenerating the pool.

| Rank | Candidate | Proposed type | Target keyword | Vol | Bucket (E/M/H · src) | Intent | Data angle | Score | Notes / angle |
|---|---|---|---|---|---|---|---|---|---|
| — | (none yet — first selection run is today's) | | | | | | | | |

---

## Coverage map (optional)

| Cluster / theme | Pieces shipped | Gaps still open |
|---|---|---|
| Book + audio identity | 1 (homepage) | site copy does not state the book relationship or credit the composer — `correct` candidate, not a new page |
| Press/retail presence | 0 | ~~inbound links from Asterism product page and publisher site — offpage brief~~ dropped 2026-09-11 (NY-4: nobody can edit those pages) |

---

## Notes

- **No duplication:** before adding a candidate, check it isn't already in `.seo/roadmap.md` or a shipped row above.
- **One piece per run.** This ledger grows by one `Shipped` row per invocation.
- **Measure before you write.** Step 0.5 reads GSC for every piece live 21+ days and updates `Performance`.
- **A page that does not map to a radar seed or a coverage-map cluster is off-topic.** The radar seeds for this site are all book/author/track phrases; a topic outside them needs a new seed first.
