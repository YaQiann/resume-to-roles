# Employer feeds, regional boards and evidence

## Employer discovery

Build a short employer list from the candidate's role families, target industries and locations. Use web search to discover employers and their official career pages; don't require the user to supply a watchlist. Work in parallel with local boards so employers using other hiring systems are not missed.

If an employer links to a public ATS board, collect that board's active postings, filter by role and location, then inspect individual links and descriptions. Verify that the board belongs to the employer before querying it. For proprietary sites or Workday use the visible official job search; don't guess private endpoints.

| Feed | Lookup | Date handling |
|---|---|---|
| [Greenhouse](https://docs.greenhouse.io/job-board.html) | Public GET `https://boards-api.greenhouse.io/v1/boards/{board_token}/jobs?content=true` | `updated_at` is an update, not original publication. |
| [Ashby](https://developers.ashbyhq.com/docs/public-job-posting-api) | Public GET `https://api.ashbyhq.com/posting-api/job-board/{board_name}` | `publishedAt` is the last publication; record that qualifier. |
| [Lever](https://github.com/lever/postings-api) | Public postings board or documented public GET; check employer region | If no reliable original date is exposed, leave it unknown. |

Use public read-only endpoints only. Send no candidate profile. Use exact board names found via employer links. Report an inaccessible feed as blocked, not as zero openings.

## Regional breadth

- Outside mainland China, prioritize accessible LinkedIn Jobs, SEEK or JobStreet where they serve the target market, and employer career pages. Search these sources in parallel where practical; supplement with country-specific boards. Do not count regional pages as coverage unless the listings actually match the target location.
- Singapore: prioritize LinkedIn Jobs, JobStreet, MyCareersFuture and employer career pages. Search local and regional variants (e.g. Singapore plus APAC/SEA) and confirm actual work location on the JD.
- Bangkok: prioritize LinkedIn Jobs, JobsDB and employer career pages, with JobThai as a supplement. Include English and local-language title variants when useful. For candidates with relevant language skills, test Mandarin/Chinese-speaking and regional variants where appropriate. Record Thai required, preferred, unstated or confirmed not required; unstated does not clear the gate.
- If an approved JobSpy installation already exists, optionally use a supported source such as Indeed for discovery. Treat its date as source-specific until independently verified. Check real links and country coverage; skip sources that are blocked. No dependency is required for this skill.

## Record evidence separately

For each candidate keep the date value, meaning (original publication, republished, updated, last refresh, first observed, or unknown), source link and observation time. An explicit original posting date in the employer's JD or structured job data is preferred. A relative date on a live detail page is usable only if its observation time and meaning establish the requested window; cached snippets and crawl timestamps do not. Resolve conflicting evidence against the employer source or mark uncertain.

Record open/current listing evidence independently of dates: current employer board membership or an explicitly active employer posting is stronger than a third-party Apply button. Exclude expired or explicitly closed jobs. Follow the [batch delivery rules](../SKILL.md#output) for counting and labeling pending candidates. A confirmed refresh or re-publication never becomes a first publication through deduplication.
