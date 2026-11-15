---
name: targeted-job-search
description: Find jobs in any profession or industry from a user's resume and target locations. Verify listings, explain fit, and deliver ranked batches of 20 without repeats.
---

# Resume to Roles

## Start with the candidate

1. If a resume is not available for this search, ask for a file or pasted text. Tell the user they can remove contact details. Reuse a resume already provided for this search.
2. Ask for target cities, broader regions or remote preferences if missing. Do not assume locations, industries or job titles.
3. Derive role families, seniority, adjacent titles, local-language synonyms and search terms from the candidate's demonstrated work, skills and stated goals. For example, a design resume may suggest product design and design systems; an operations resume may suggest business operations and program management; an engineering resume may suggest roles by technical specialty and level. Examples are not default tracks. Record unknown constraints without inventing them.

## Find and verify

**Search narrow to wide.** Aim for 20 unseen, dated candidates in each of the first two batches from the last 7 days, expanding to 10 days if needed. Before using older dates, reuse unseen candidates, vary relevant keywords, paginate and search additional appropriate platforms in the same geography. Only when these routes are exhausted or blocked, widen to 15 days and then 20 days if still short. Keep all 7–10-day candidates ahead of wider-window additions, label the widened tier and explain the coverage gap. Apply the same sequence on later batches; do not change the location without user direction.

Search multiple relevant role families on local boards and directly on employers' career sites. Use [source routing and date rules](references/search-sources.md) for employer feeds, Singapore and Bangkok. For mainland China, search BOSS直聘, 猎聘 and LinkedIn first; use [China portal search](references/china-portals.md). Start with the last 7 calendar days including today, in the user's timezone; if fewer than 20 worthwhile candidates are found, expand to 10 days. Try additional role synonyms, in-scope sources and result pages before returning a short batch; stop when available coverage is exhausted or blocked, or two passes yield no relevant new candidates.

Open individual descriptions for promising roles. Record employer, title, location, direct link, source, job ID, posting-date evidence, status and disclosed pay. Treat first publication, refresh dates and hiring status separately. A list card, crawl date or Apply button alone does not establish current availability. Label missing dates, uncertain status and partial descriptions separately.

Check explicit requirements first: work location, language, work authorization, licenses and other mandatory credentials. Mark each as met, unmet or unknown. Exclude known hard failures from recommendations. Rank using evidence for responsibilities, skills, seniority and domain; distinguish direct matches, transferable experience and gaps. Match the actual work, not just title or tools: a shared SQL keyword does not establish investment-domain or data-engineering fit. Treat preferences differently from mandatory requirements. Do not invent skills or treat a match score as interview odds.

## Output

Finish an initial pass on all priority sources before selecting the 20, even if one source alone already yields 20. Rank the merged pool; carry over unshown candidates. Keep each platform’s date evidence when merging a duplicate, rather than replacing an original date with a newer refresh.

For the dated batch, count eligible recent original postings and recent refreshes (label each distinctly); unclear hiring status or partial JD does not disqualify a candidate that has a reliable date, direct link and visible fit evidence. Keep undated leads outside the 20 count. This narrow-to-wide policy overrides any more permissive lead inclusion guidance below.

**Default: 20 distinct worthwhile candidates per batch.** Rank worthwhile candidates in this order: original publication within the window, then a verified refresh or update within the window when no recent original publication is established, then other promising date-unverified leads in a separate section. Rank by fit within each section. Both recent groups count toward 20; keep date-unverified leads separate and outside the 20 count. Label each date as 首发, 刷新/更新, or 日期待核实. A known older original date does not disqualify a recently refreshed role unless it is explicitly closed or expired. Pending candidates need a direct job link and enough visible fit evidence. List-only leads without a direct job link are separate and do not count. Exclude closed, expired, duplicate or irrelevant jobs, and old postings without recent activity from the dated groups. Report total and split (e.g. 20 candidates: 6 verified, 14 pending), and explain any shortfall after searching available sources. Number rows across both groups and use:

| # | 地点 | 岗位 | 为什么值得看 | 还需确认 |
|---|---|---|---|---|
| 1 | 城市 | 公司、职位直链、发布日期证据、已披露薪资 | 具体职责对应的简历证据 | 最大差距或尚未核实的门槛 |

Summarize sources checked, unique leads, individual descriptions actually read, verified matches and access limits. Track summary-only, blocked and closed separately; blocked does not mean closed or zero results. Ask which roles are worth pursuing. On “下一批” or “都不合适”, reuse the candidate profile and search scope, apply explicit feedback, and search for the next 20. Keep a session ledger of source/query/city, last completed page or cursor, access status, candidate identities, and shown IDs (including unverified leads). Reuse unseen eligible candidates before fetching more pages. Deduplicate by employer-scoped requisition ID, normalized URL and equivalent employer/title/location; preserve separate requisitions when evidence shows they differ. Recruiter listings can be candidate duplicates even when boards format the title differently; compare agency, contract duration, location and public reference, and flag uncertainty if the end employer is unknown. When a shown lead is verified later, report it as an update rather than counting it again. For optional persistence, use a user-approved private location outside this skill directory.

Use role and location keywords only when querying job sources; do not send the resume, contact details or credentials to job boards. Never package candidate files, profiles, search logs, feedback or credentials with the skill. Do not auto-apply, send messages or schedule searches without authorization.
