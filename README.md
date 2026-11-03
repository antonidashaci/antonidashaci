<!-- Replace the heading with your real name — clients hire a person, not a handle. -->
# antonidashaci

I make games, and I build backend and tooling to pay for making games.
Python and FastAPI on the server, TypeScript on the front end, C++ and C# in
engines. Open to freelance work in Turkish or English.

## Games

This is the main thing. Two of them aren't public yet.

**Anomaly Corridor** — Horror game in Unreal, C++. Levels and art are built by
a generation pipeline rather than placed by hand, so the layout differs per
run. Still in development; the repo is private for now.

**Pantheon Everlust** — Gacha RPG in Unity. C# on the client, TypeScript
service behind it for accounts and the pull logic. In development, private.

**[match3](https://github.com/antonidashaci/match3)** — Match-3 puzzle game in
Next.js and React. Not just the board: level map, shop, daily wheel, rewards,
sound and settings, so the whole loop is there.

**[oyalanmaca](https://github.com/antonidashaci/oyalanmaca)** — Trivia game in
Flutter. Twenty questions, five seconds each, lives you can refill, daily
streaks, and a Wordle-style emoji grid for sharing a result.

**[ai-rpg-alpha](https://github.com/antonidashaci/ai-rpg-alpha)** — Text RPG
engine in Python. Turn-based combat, long multi-act quests, six schools of
magic, NPCs with branching dialogue, and three kingdoms whose opinion of you
changes with what you do.

## Command-line tools

Python, one file each, standard library only. Download and run.

| | |
| --- | --- |
| **[envdiff](https://github.com/antonidashaci/envdiff)** | Compares two `.env` files and exits non-zero when a key is missing or empty. Meant for CI. |
| **[csvpeek](https://github.com/antonidashaci/csvpeek)** | Prints what's actually in a CSV: column types, how many nulls, numeric ranges, the common values. |
| **[dupefind](https://github.com/antonidashaci/dupefind)** | Finds duplicate files by content, in three passes so most files never get opened. Deletes nothing. |
| **[cronreader](https://github.com/antonidashaci/cronreader)** | Says what a cron expression means in plain English and prints the next times it fires. |
| **[secretscan](https://github.com/antonidashaci/secretscan)** | Looks for API keys and passwords about to be committed. Runs as a pre-commit hook. |
| **[logstats](https://github.com/antonidashaci/logstats)** | Turns an nginx or Apache access log into a readable report: errors, slowest paths, top clients. Reads `.gz`. |
| **[imgsqueeze](https://github.com/antonidashaci/imgsqueeze)** | Resizes and compresses a folder of images for the web. Dry run unless you say otherwise. |
| **[sitemapper](https://github.com/antonidashaci/sitemapper)** | Crawls a site and writes `sitemap.xml`. Follows robots.txt and canonical tags. |

## APIs

| | |
| --- | --- |
| **[url-shortener-api](https://github.com/antonidashaci/url-shortener-api)** | URL shortener. FastAPI and SQLite in one file, no ORM. Random slugs, expiry, click counts. |
| **[webhook-inspector](https://github.com/antonidashaci/webhook-inspector)** | Catches webhooks so you can read them, then replays them at your local server as often as you need. Useful when wiring up Stripe. |

## JavaScript libraries

No dependencies, ESM, tested with `node --test`.

| | |
| --- | --- |
| **[slugify-tr](https://github.com/antonidashaci/slugify-tr)** | Slugify that gets Turkish ı and İ right. Most libraries turn "İstanbul" into "i̇stanbul". |
| **[fetch-retry-lite](https://github.com/antonidashaci/fetch-retry-lite)** | `fetch` with backoff and `Retry-After`. Won't retry a POST unless you ask, because a timed-out POST may already have charged the card. |
| **[money-fmt](https://github.com/antonidashaci/money-fmt)** | Money kept as integer minor units. Formats per locale and parses it back, which `Intl` won't do. |
| **[tiny-validate](https://github.com/antonidashaci/tiny-validate)** | Schema validation you compose. Errors carry the field path, so a 422 can say which field is wrong. |
| **[lazy-img](https://github.com/antonidashaci/lazy-img)** · [demo](https://antonidashaci.github.io/lazy-img/demo.html) | Custom element for lazy images. Holds its space so the page doesn't jump, builds a `srcset`, retries a failed load. |

## Web apps

No build step, no server, nothing leaves the browser. Click a demo and use it.

| | |
| --- | --- |
| **[jwt-peek](https://antonidashaci.github.io/jwt-peek/)** | Decode a JWT and check its signature without pasting it into someone else's site. |
| **[palette-lab](https://antonidashaci.github.io/palette-lab/)** | Build a colour ramp and see which shades are readable as body text. |
| **[invoice-maker](https://antonidashaci.github.io/invoice-maker/)** | Fill in an invoice and print it to PDF. VAT grouped per rate. |
| **[markdown-notes](https://antonidashaci.github.io/markdown-notes/)** | Markdown notes with live preview, stored on your machine. |
| **[expense-splitter](https://antonidashaci.github.io/expense-splitter/)** | Work out who owes whom after a shared trip, in as few transfers as possible. |
| **[pomodoro-focus](https://antonidashaci.github.io/pomodoro-focus/)** | Pomodoro timer that's still right after an hour in a background tab. |

## Other things I've built

**[fintechhub](https://github.com/antonidashaci/fintechhub)** — Comparison site
for Turkish banks and fintech products. Multi-page, blog, provider pages.

**[karala](https://github.com/antonidashaci/karala)** — Blurs names, IBANs and
faces out of a screenshot before you send it. Runs entirely on the phone;
nothing is uploaded. Web core wrapped with Capacitor for Play Store.

**[botv2](https://github.com/antonidashaci/botv2)** — Python bot, packaged and
tested.

## How I work

Most of these have no dependencies, because a dependency is someone else's
decision you inherit. The ones that do use FastAPI or Pillow, where writing it
myself would be silly.

Tests go where things break: timezones, rounding, money, dates, strings in
languages that aren't English. All of it runs in CI.

## Contact

<!-- Put your email and profile links here. -->
Open an issue on any repo.
