# Emre Cihangir

I build small, sharp tools: Python CLIs and APIs, and vanilla-JS libraries and
web apps. Available for freelance work — Turkish and English.

Everything below is public, tested in CI, and written to the same standard: no
dependencies unless they earn their place, a README that explains the problem
before the API, and tests that cover the cases that actually break.

**41 repositories · 911 tests · no dependencies in 35 of them**

---

## Developer tools (Python, CLI)

Single file, standard library only, drop it in and run it.

| | What it does | Why it's interesting |
| --- | --- | --- |
| **[envdiff](https://github.com/antonidashaci/envdiff)** | Compare two dotenv files, exit non-zero on a missing key | Turns "works on my machine" into a build failure instead of a 500 |
| **[csvpeek](https://github.com/antonidashaci/csvpeek)** | Summarise a CSV: types, null rates, ranges, top categories | `head` shows rows; before writing import code you want the *shape* |
| **[dupefind](https://github.com/antonidashaci/dupefind)** | Find duplicate files by content | Three passes, cheapest first — a file with a unique size is never opened. Never deletes anything |
| **[cronreader](https://github.com/antonidashaci/cronreader)** | Explain a cron expression and print its next runs | Gets the real rule that day-of-month and day-of-week are OR'd |
| **[secretscan](https://github.com/antonidashaci/secretscan)** | Catch committed API keys and DB passwords | 13 rules, three layers of false-positive filtering, findings redacted in output |
| **[logstats](https://github.com/antonidashaci/logstats)** | nginx/Apache access log → a report you can read | p95 per path, top errors, top clients. Reads `.gz` and pipes |
| **[imgsqueeze](https://github.com/antonidashaci/imgsqueeze)** | Batch-resize and compress images for the web | Dry run by default, strips EXIF, honours rotation, never upscales |
| **[sitemapper](https://github.com/antonidashaci/sitemapper)** | Crawl a site, write `sitemap.xml` | Canonical-aware, respects robots.txt, one URL per page instead of five spellings |
| **[migrate-guard](https://github.com/antonidashaci/migrate-guard)** | Catch the Postgres migration that will lock a table in production | Fails CI before it ships. The SQL is parsed, not regexed — dollar quotes included |
| **[importcycle](https://github.com/antonidashaci/importcycle)** | Circular imports, layering violations and dead modules in a package | Found statically, without importing anything — so a cycle can't crash the checker |
| **[flakyfind](https://github.com/antonidashaci/flakyfind)** | Name the flaky tests from the JUnit XML your CI already writes | Won't quarantine a test that is simply broken — same failure every run is not flake |
| **[slowquery](https://github.com/antonidashaci/slowquery)** | Group a Postgres slow query log by shape and propose the index | Ranked by **total** time, not worst case: 10,000 queries at 40ms beat one at 9s |
| **[tracegroup](https://github.com/antonidashaci/tracegroup)** | Group stack traces in a log and fail a deploy on a **new** error | Handles frame order being reversed between Python and the JVM/V8 |
| **[idpeek](https://github.com/antonidashaci/idpeek)** | Paste an id, find out what it leaks | A UUIDv1 carries a MAC address and a timestamp; a snowflake carries a date |
| **[apidiff](https://github.com/antonidashaci/apidiff)** | Diff two OpenAPI specs, fail the build on a breaking change | Requests and responses break in opposite directions — most diff tools get this backwards |

## APIs (FastAPI + SQLite, one file each)

| | |
| --- | --- |
| **[url-shortener-api](https://github.com/antonidashaci/url-shortener-api)** | Random slugs (not enumerable ids), `http(s)`-only targets, 307 so clicks keep counting, expiry → 410 |
| **[webhook-inspector](https://github.com/antonidashaci/webhook-inspector)** | Catch webhooks, read them in a live page, and **replay them at `localhost`** — verbatim, signature header included |
| **[feature-flag-api](https://github.com/antonidashaci/feature-flag-api)** | Percentage rollouts that **stay stable when you change the percentage** — hashed buckets, not `random()`, so nobody gets reshuffled at 10% → 20% |
| **[job-queue-api](https://github.com/antonidashaci/job-queue-api)** | A crash-safe queue on SQLite: the lease is a row with an expiry, so an OOM-killed worker's job comes back by itself. Backoff, priorities, dead-letter revive |
| **[audit-log-api](https://github.com/antonidashaci/audit-log-api)** | An audit log you can prove nobody edited — each entry hash-chained to the last, so a deleted or altered row breaks verification |

## JavaScript libraries

Zero dependencies, ESM, tested with `node --test`.

| | What it does | Why it exists |
| --- | --- | --- |
| **[slugify-tr](https://github.com/antonidashaci/slugify-tr)** | Turkish-aware slugify | `'İstanbul'.toLowerCase()` is 9 code points, not 8 — a combining dot you didn't ask for |
| **[fetch-retry-lite](https://github.com/antonidashaci/fetch-retry-lite)** | `fetch` + backoff, jitter, `Retry-After` | Never retries POST by default: a timed-out POST may have succeeded, and retrying charges the card twice |
| **[money-fmt](https://github.com/antonidashaci/money-fmt)** | Integer-minor-unit money, format **and parse** | `Intl` formats but won't parse, and `0.1 + 0.2` is how invoices go wrong by a kurus |
| **[tiny-validate](https://github.com/antonidashaci/tiny-validate)** | Composable schema validation | Every error carries the field path, so a 422 can tell the client what to fix |
| **[lazy-img](https://github.com/antonidashaci/lazy-img)** · [demo](https://antonidashaci.github.io/lazy-img/demo.html) | Lazy responsive `<lazy-img>` element | Reserves its own space, generates a `srcset`, retries failures — the half `loading="lazy"` doesn't cover |
| **[recurring](https://github.com/antonidashaci/recurring)** | Expand an RFC 5545 `RRULE` in a real time zone | A 09:00 weekly meeting is still at 09:00 after the clocks change |
| **[async-pool](https://github.com/antonidashaci/async-pool)** | Async work with a concurrency limit | Results in **input** order though completion isn't, lazy sources, `AbortSignal` |
| **[fuzzy-find](https://github.com/antonidashaci/fuzzy-find)** | Typo-tolerant search for a palette or a 50,000-row filter | The highlight offsets are the ones that actually matched, not a second guess |
| **[tr-doc](https://github.com/antonidashaci/tr-doc)** | Turkish identifiers by their real checksums — TCKN, tax number, IBAN, plate, phone | Returns *why* it failed, so a form can say something useful |
| **[text-diff](https://github.com/antonidashaci/text-diff)** | Myers diff, word-level refinement, unified output, and a patcher | The patcher verifies context before it writes — a stale patch is refused, not half-applied |

## Web apps

Local-first, no build step, no server, dark mode. Click a demo and use it.

| | | |
| --- | --- | --- |
| **[jwt-peek](https://github.com/antonidashaci/jwt-peek)** | [demo](https://antonidashaci.github.io/jwt-peek/) | Decode and check a JWT **offline**. Won't let the token choose its own verification algorithm |
| **[palette-lab](https://github.com/antonidashaci/palette-lab)** | [demo](https://antonidashaci.github.io/palette-lab/) | Colour ramps spaced by WCAG luminance, not HSL — and which shades pass for body text |
| **[invoice-maker](https://github.com/antonidashaci/invoice-maker)** | [demo](https://antonidashaci.github.io/invoice-maker/) | Invoice → PDF. VAT grouped per rate, the way a return is filed |
| **[markdown-notes](https://github.com/antonidashaci/markdown-notes)** | [demo](https://antonidashaci.github.io/markdown-notes/) | Notes with a markdown renderer written from scratch — safe by construction, not by filtering |
| **[expense-splitter](https://github.com/antonidashaci/expense-splitter)** | [demo](https://antonidashaci.github.io/expense-splitter/) | Split a bill into the fewest transfers that settle it, losing no kurus |
| **[pomodoro-focus](https://github.com/antonidashaci/pomodoro-focus)** | [demo](https://antonidashaci.github.io/pomodoro-focus/) | Still correct after an hour in a background tab, because it reads the clock instead of counting ticks |
| **[regex-lab](https://github.com/antonidashaci/regex-lab)** | [demo](https://antonidashaci.github.io/regex-lab/) | Explain a pattern, and count the backtracking **in steps** — so the ReDoS answer is the same on every machine. Own engine; your pattern never reaches `RegExp` |
| **[cert-peek](https://github.com/antonidashaci/cert-peek)** | [demo](https://antonidashaci.github.io/cert-peek/) | X.509 parsed by hand from ASN.1/DER in the tab — because pasting a certificate into a website is how a private key leaks |
| **[pass-check](https://github.com/antonidashaci/pass-check)** | [demo](https://antonidashaci.github.io/pass-check/) | `Istanbul2024!` is not strong. Scores the **cheapest** way in — words, dates, keyboard walks — with a Turkish word list |
| **[qr-forge](https://github.com/antonidashaci/qr-forge)** | [demo](https://antonidashaci.github.io/qr-forge/) | A QR encoder written out step by step — Reed-Solomon, masks, penalty rules — with a decoder that reads it back to prove it |
| **[tz-meet](https://github.com/antonidashaci/tz-meet)** | [demo](https://antonidashaci.github.io/tz-meet/) | Meeting times across zones from the platform's own IANA data: +05:45, half-hour DST shifts, and a warning when someone's clocks change mid-range |

---

## How I work

- **The problem first.** Every README opens with the bug the code exists to
  prevent, not with an API table.
- **Dependencies have to earn it.** 35 of these 41 repos have none. The
  exceptions are FastAPI and Pillow, where writing it myself would be silly.
- **Tests cover what breaks**, not what's easy: timezone edges, float drift,
  rounding against a tax authority's method, XSS payloads, clocks jumped
  forward by a year, a tab suspended for an hour.
- **Safety isn't a filter.** Order the code so the unsafe state can't exist —
  escape before you build the tag, pass the algorithm in rather than reading it
  from the token.
- **Rounding, dates and money are where projects actually go wrong**, so those
  get the most attention and the most tests.

## Stack

Python · FastAPI · SQLite · JavaScript (ESM) · Web Components · HTML/CSS ·
Git · GitHub Actions

## Get in touch

- Bionluk (freelance, TR): https://bionluk.com/emre_cihangir
- Or open an issue on any repo.

<!-- Add e-mail / LinkedIn / Upwork here when you want them public. -->
