<!-- Add your name to the heading below, and your contact details at the bottom. -->
# Hi there

I build small, sharp tools: Python CLIs and APIs, and vanilla-JS libraries and
web apps. Available for freelance work — Turkish and English.

Everything below is public, tested in CI, and written to the same standard: no
dependencies unless they earn their place, a README that explains the problem
before the API, and tests that cover the cases that actually break.

**21 repositories · 307 tests · no dependencies in 17 of them**

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

## APIs (FastAPI + SQLite, one file each)

| | |
| --- | --- |
| **[url-shortener-api](https://github.com/antonidashaci/url-shortener-api)** | Random slugs (not enumerable ids), `http(s)`-only targets, 307 so clicks keep counting, expiry → 410 |
| **[webhook-inspector](https://github.com/antonidashaci/webhook-inspector)** | Catch webhooks, read them in a live page, and **replay them at `localhost`** — verbatim, signature header included |

## JavaScript libraries

Zero dependencies, ESM, tested with `node --test`.

| | What it does | Why it exists |
| --- | --- | --- |
| **[slugify-tr](https://github.com/antonidashaci/slugify-tr)** | Turkish-aware slugify | `'İstanbul'.toLowerCase()` is 9 code points, not 8 — a combining dot you didn't ask for |
| **[fetch-retry-lite](https://github.com/antonidashaci/fetch-retry-lite)** | `fetch` + backoff, jitter, `Retry-After` | Never retries POST by default: a timed-out POST may have succeeded, and retrying charges the card twice |
| **[money-fmt](https://github.com/antonidashaci/money-fmt)** | Integer-minor-unit money, format **and parse** | `Intl` formats but won't parse, and `0.1 + 0.2` is how invoices go wrong by a kurus |
| **[tiny-validate](https://github.com/antonidashaci/tiny-validate)** | Composable schema validation | Every error carries the field path, so a 422 can tell the client what to fix |
| **[lazy-img](https://github.com/antonidashaci/lazy-img)** · [demo](https://antonidashaci.github.io/lazy-img/demo.html) | Lazy responsive `<lazy-img>` element | Reserves its own space, generates a `srcset`, retries failures — the half `loading="lazy"` doesn't cover |

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

---

## How I work

- **The problem first.** Every README opens with the bug the code exists to
  prevent, not with an API table.
- **Dependencies have to earn it.** 17 of these 21 repos have none. The
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

Open an issue on any repo.

<!-- Add the rest when you're ready, e.g.:
Email: you@example.com · Upwork: … · LinkedIn: … · Bionluk: …
-->

