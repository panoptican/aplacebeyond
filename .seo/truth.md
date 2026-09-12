# Source of truth

Derived from the repo and the book's public product page. This is what fact-check prompts are scored against.
Re-derive whenever the book's product data, the site copy, or the track changes. A stale truth file turns
correct answers into false accuracy failures.

## The work

| Claim | Value | Source | Read |
|---|---|---|---|
| Book title | A Place Beyond | asterismbooks.com/product/a-place-beyond | 2026-09-11 |
| Book author | Garett Strickland | same | 2026-09-11 |
| Book designer | Mike Corrao | same | 2026-09-11 |
| Publisher | Inside the Castle | same ("from Inside the Castle") | 2026-09-11 |
| Retailer | Asterism Books | same | 2026-09-11 |
| Retail price | $50.00 USD | same | 2026-09-11 |
| Format | Paperback, full color, 336 pages, 7.75"x9.5"x0.88", 29 oz | same | 2026-09-11 |
| ISBN-13 | 9798987083895 | same | 2026-09-11 |
| Preorder note | Signed by the author + original work of art | same (verify before restating) | 2026-09-11 |
| Related work | Ungula — diptych partner ("the former dwells…the latter lies beyond the portal") | Logan Berry blurb, same page | 2026-09-11 |
| Public blurbs | Logan Berry; Jake Reber | same | 2026-09-11 |
| Track on site | "Blackmoon" (blackmoon.mp3) | repo: index.html | 2026-09-11 |
| Track author | Garett Strickland (composed for the book, not licensed) | owner interview | 2026-09-11 |
| Site designer | Jason Spidle | owner interview | 2026-09-11 |
| Site purpose | Audio accompaniment to the book | owner interview; not yet stated on the site | 2026-09-11 |
| Site canonical URL | https://aplacebeyond.place/ | repo: index.html | 2026-09-11 |
| Site price | Free, no accounts, no e-commerce | repo: index.html (no store code) | 2026-09-11 |

## Integrations / presence

Include the negatives. "We do not integrate with X" is the claim an engine is most
likely to get wrong in the flattering direction.

| Presence | Status | Source |
|---|---|---|
| Bandcamp page for the track | unknown — not evidenced | web search 2026-09-11 found none |
| Spotify / Apple Music release | unknown — not evidenced | web search 2026-09-11 found none |
| Audio download on-site | no (controlsList="nodownload") | repo: index.html |
| Mailing list / accounts | no | repo: index.html |
| llms.txt | no | repo listing |

## Contradictions found

Where surfaces disagree. Each of these is already a finding: if your own surfaces
contradict each other, an engine synthesizing both produces a muddle.

| Claim | Code says | Site says | Which is right |
|---|---|---|---|
| What the site is | Purpose is "audio accompaniment to the book A Place Beyond" (owner, 2026-09-11) | "immersive ambient music experience featuring cinematic visuals and the original track Blackmoon" — the book is never mentioned; author never named | The book relationship is the truth; the site copy is incomplete, not wrong |
| Track authorship | Garett Strickland composed "Blackmoon" (owner) | "the original track Blackmoon" — no composer credit | Composer credit belongs on the page (author of the book, creator of the music) |
| "Blackmoon" casing | "Blackmoon" (file, meta, JSON-LD) | "Blackmoon" | consistent |

## HIGH-RISK

None regulatory, medical, legal, or financial. The nearest risk: misattributing the
work (author/composer/publisher). Every create and refresh action must keep the
attribution chain exact: Garett Strickland (author + music), Mike Corrao (designer),
Inside the Castle (publisher), Asterism Books (retailer).
