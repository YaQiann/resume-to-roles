# BOSS直聘 and 猎聘

These are read-only discovery sources. Do not request passwords, cookies or verification codes, or click communication, application or resume controls.

## 猎聘: use the upstream CLI when available

Use a user-approved local checkout of [ai-job-search-cn](https://github.com/rockbenben/ai-job-search-cn). Inspect code before first use. If the checkout is unavailable, use public search; do not silently install software. Node 22.18+ is sufficient for this module.

From upstream's root, run the documented search and detail commands with the user's city and role terms:

```sh
node .agents/skills/liepin-search/cli/src/cli.ts search -q "<关键词>" -l "<城市>" --limit 12 --format json
node .agents/skills/liepin-search/cli/src/cli.ts detail "<职位直链>" --format plain
```

Use returned `meta.hasNext` and `--page` for later batches, provided the applicable usage rules allow the access. Keep the returned direct URL (enterprise and headhunter URLs differ). The CLI search `date` is derived from `refreshTime`: record it as **refresh date**, never original publication date. Do not use the search date filter as evidence of an original 7–10-day posting window. If full detail cannot establish publication date, list it as date-unverified.

## BOSS直聘: use the visible site search

Borrow the browser workflow, not proprietary network calls. When the user's browser can be used, start from the actual BOSS tab and search via visible keyword and city controls. Use the user's existing signed-in tab if needed; if search navigation leaves BOSS, ask the user to open the desired result page and resume from that tab. Open promising job cards and record the individual job URL and visible JD. Use visible next-page or load-more controls if present. Stop on verification or access limits and let the user handle verification.

If browser access is unavailable, use a public BOSS search with city + role keywords. Follow individual job links when available; otherwise record title, company, listed salary, city and list source as a **listing-only lead**. A search index hit is not a verified live opening. Don't claim authenticated coverage unless a detail was actually read in that session.

## Merge and continue

Track platform, city, keyword and page, then deduplicate across sources by posting ID/URL and equivalent company + role + city. Preserve both sources when merged. Follow the [main skill's batch rules](../SKILL.md#output) for the 20-job target, date verification and “下一批”.
