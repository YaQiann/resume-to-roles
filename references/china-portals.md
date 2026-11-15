# BOSS直聘 and 猎聘

These are read-only discovery sources. Do not request passwords, cookies or verification codes, or click communication, application or resume controls.

## 猎聘: use the upstream CLI when available

Use a user-approved local checkout of [ai-job-search-cn](https://github.com/rockbenben/ai-job-search-cn). Inspect code before first use. If the checkout is unavailable, use public search; do not silently install software. Node 22.18+ is sufficient for this module.

From upstream's root, run the documented search and detail commands with the user's city and role terms:

```sh
node .agents/skills/liepin-search/cli/src/cli.ts search -q "<关键词>" -l "<城市>" --limit 12 --format json
node .agents/skills/liepin-search/cli/src/cli.ts detail "<职位直链>" --format plain
```

Use returned `meta.hasNext` and `--page` for later batches, provided the applicable usage rules allow the access. Keep the returned direct URL (enterprise and headhunter URLs differ). The CLI search `date` is derived from `refreshTime`: record it as **refresh date**, never original publication date. Do not use the search date filter as evidence of an original 7–10-day posting window. If original publication is unknown, retain a reliable recent refresh as a dated fallback candidate and label it 刷新; never mark it 首发. Also search LinkedIn public job pages in parallel for mainland China and apply the same date rules.

## BOSS直聘: use the visible site search

Borrow the browser workflow, not proprietary network calls. When the user's browser can be used, start from the actual BOSS tab and search via visible keyword and city controls. Use the user's existing signed-in tab if needed; if search navigation leaves BOSS, ask the user to open the desired result page and resume from that tab. Open promising job cards and record the individual job URL and visible JD. Use visible next-page or load-more controls if present. Stop on verification or access limits and let the user handle verification.

If browser access is unavailable, use a public BOSS search with city + role keywords. Follow individual job links when available; otherwise record title, company, listed salary, city and list source as a **listing-only lead**. A search index hit is not a verified live opening. Don't claim authenticated coverage unless a detail was actually read in that session.

Track progress separately as page opened, result list read, and individual JD read. If verification interrupts the browser, keep candidates already read, continue the other sources, and tell the user which search page to reopen or verify manually. Do not retry blocked pages in a loop. Recruiter activity and listing refresh are not publication dates.

## Merge and continue

For mainland China, make an initial search pass on BOSS, Liepin and LinkedIn before finalizing each batch. Do not stop at 20 from the first source. Check promising matches from every accessible source; record unavailable sources and continue. Pool candidates before ranking so stronger or newer postings from later sources can replace weaker ones.

For the same job across platforms, display one row and preserve per-source links, date values, date types and hiring-status evidence. Do not collapse an original date and a refresh date into one generic date (e.g. LinkedIn 首发 11/10 · 猎聘刷新 11/13, when both types are supported by evidence). If first-publication claims conflict, prefer explicit employer evidence or label the conflict unresolved. Use the clearest direct application link and retain useful alternative links.

Track platform, city, keyword and page, then deduplicate across sources by posting ID/URL and equivalent company + role + city. Preserve both sources when merged. Follow the [main skill's batch rules](../SKILL.md#output) for the 20-job target, date verification and “下一批”.
