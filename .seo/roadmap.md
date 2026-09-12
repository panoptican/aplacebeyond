# A Place Beyond — Roadmap

> **Canonical document** for programmatic work. This site is a single-book companion: the standard programmatic patterns (alternatives, compare, use-case, playbook) do not apply and are intentionally absent. The roadmap here tracks the honest phases a one-page book site actually needs.

---

## Phase Status Tracker

| # | Phase | Pattern | Status | PR |
|---|---|---|---|---|
| 0 | Technical foundations | Setup | in_progress | – |
| 1 | State the book relationship on-page | fix (correct) | pending | – |
| 2 | Inbound links: Asterism product page + publisher | offpage | dropped (NY-4: nobody can edit those pages) | – |

**Conventions:**
- `pending` → `in_progress` (when worktree starts) → `completed` (in same commit as PR)
- PR column: `branch \`name\` (PR TBD)` then update to `#NNN` after `gh pr create`

---

## Reference Data (read once per agent)

### 1. Site facts

- **Domain:** https://aplacebeyond.place
- **GSC property:** connected by user (2026-09-11, NY-1 closed); host-side client credentials still missing
- **Bing site:** not connected
- **OpenSEO project:** not connected
- **Authority / playable bucket:** unknown → easy (no tools, no rankings; as of 2026-09-11)
- **Stack:** static HTML (Cloudflare Pages via wrangler.toml, `pages_build_output_dir = "."`)
- **Brand accent color:** #959588 on #0B0902
- **Hero font / body font:** system defaults
- **Marketing pages root:** repo root (`index.html`)

### 2. Existing programmatic surface (DO NOT DUPLICATE)

None — and none planned.

### 3. Critical files

| File | What lives there |
|---|---|
| `index.html` | The only page: video background, audio player, all metadata and JSON-LD |
| `robots.txt` | Allow all + sitemap reference |
| `sitemap.xml` | Single URL (homepage) |
| `wrangler.toml` | Cloudflare Pages config |
| `blackmoon.mp3` | The track |
| `generativeBG.mp4` | The video background |

### 4. Data shapes

n/a — no programmatic patterns on this site.

### 5. Conventions

**URL slugs:** lowercase, hyphenated, never underscored.

**The book relationship is non-negotiable on-page:** every page must be legible as the audio accompaniment to *A Place Beyond* by Garett Strickland. Attribution chain: Garett Strickland (author + music), Mike Corrao (designer), Inside the Castle (publisher), Asterism Books (retailer).

---

## Keyword Research Appendix

No keyword tools connected. Seed terms from the owner interview (2026-09-11) — volumes unknown until a tool or GSC is connected:

### A.1 — Brand terms (must rank #1; site's whole job)

- "A Place Beyond" (book)
- "A Place Beyond Garett Strickland"
- "Blackmoon Garett Strickland"
- "A Place Beyond audio"

### A.2 — Topic terms the site could plausibly serve

- "ambient music for reading"
- "music to listen to while reading"
- "asemic writing"
- "experimental literature audio"

### A.3 — Already-saturated head terms (avoid)

- "ambient music" (generic; site is not a platform)
- "Inside the Castle press" (publisher's term)

### A.4 — Out of scope (intentionally excluded)

- Reviews/analysis of the book (not this site's job)
- Streaming playlists, download packs, merch, events

---

## Phases

### Phase 0 — Technical foundations

**Why:** the site is 7 months old with one page. Get the basics verified before anything else.

**Scope:**
1. Verify sitemap.xml + robots.txt are correct and served (done in repo; verify live)
2. Confirm title + description on the single page are unique and indexable (present; will change in Phase 1)
3. Schema: MusicRecording JSON-LD already present — verify it validates
4. Submit sitemap in GSC + Bing once connected (manual, NY-1)

**Verification:**
- [ ] `tech_audit.py` returns 0 critical findings
- [ ] Sitemap submitted in GSC (manual, blocked on NY-1)

### Phase 1 — State the book relationship on-page

**Why:** the site currently presents as a generic ambient page. Engines (and readers who land from search) cannot learn that this is the audio accompaniment to the book, who made it, or where to buy the book. That is the whole relevance story.

**Scope (draft — the fix lane owns the details):**
1. Title/meta: mention the book and author
2. On-page copy (sparse, matching voice): book relationship, composer credit, artist/author line, link out to the Asterism product page
3. Extend JSON-LD: MusicRecording byArtist Garett Strickland; WebSite description states the book relationship

**Verification:** `truth_check.py` passes (composer credited, book relationship stated).

### Phase 2 — Inbound links — DROPPED

**Dropped 2026-09-11 (NY-4):** nobody can edit the Asterism product page or the publisher site, so no offpage brief can be sent. Keep an eye out — if the publisher ever asks for assets, resurrect this phase.

**Why it would have mattered:** the highest-authority pages about this book (Asterism product page, publisher site) currently do not link to the companion site. One link from each is worth more than any content work.

**Scope:** offpage brief asking the publisher to link the companion site from the book's pages. A human sends it.

---

## Off-page checklist

- [ ] ~~Ask publisher/author to add aplacebeyond.place link to the Asterism product page (via publisher)~~ dropped 2026-09-11 (NY-4: nobody can)
- [ ] Publisher site (insidethecastle.org) mention on the book page — same brief
- [ ] (optional) Author's own profiles — same brief
- No paid directories — not applicable to this site

## Glossary

- **Bucket** — Easy / Medium / Hard winnability read. This site starts at easy.
- **KD** — keyword difficulty; no vendor connected, so no numbers exist yet.
