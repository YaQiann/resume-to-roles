---
name: targeted-job-search
description: Find jobs in any profession or industry from a user's resume and target locations. Verify listings, explain fit, and deliver ranked batches of 20 without repeats.
---

# Targeted job search

## Start with the candidate

1. If a resume is not available for this search, ask for a file or pasted text. Tell the user they can remove contact details. Reuse a resume already provided for this search.
2. Ask for target cities, broader regions or remote preferences if missing. Do not assume locations, industries or job titles.
3. Derive role families, seniority, adjacent titles, local-language synonyms and search terms from the candidate's demonstrated work, skills and stated goals. For example, a design resume may suggest product design and design systems; an operations resume may suggest business operations and program management; an engineering resume may suggest roles by technical specialty and level. Examples are not default tracks. Record unknown constraints without inventing them.

## Find and verify

Search multiple relevant role families on employer sites and suitable local or specialist job boards. For BOSS直聘 and 猎聘, use [China portal search](references/china-portals.md). Start with the last 7 days; if fewer than 20 qualify, expand to 10 days. Try additional role synonyms, in-scope sources and result pages before returning a short batch; stop when available coverage is exhausted or blocked, or two passes yield no relevant new candidates.

Open individual descriptions for promising roles. Record employer, title, location, direct link, source, job ID, posting-date evidence, status and disclosed pay. Treat first publication, refresh dates and hiring status separately. A list card, crawl date or Apply button alone does not establish current availability. Keep high-match leads with unverified dates or status separate from the verified batch.

Check explicit requirements first: work location, language, work authorization, licenses and other mandatory credentials. Mark each as met, unmet or unknown. Exclude known hard failures from recommendations. Rank using evidence for responsibilities, skills, seniority and domain; distinguish direct matches, transferable experience and gaps. Do not invent skills or treat a match score as interview odds.

## Output

**Default: 20 distinct recommendations per batch, ranked by fit.** If fewer qualify after reasonable coverage, report the actual count and why. Do not pad with stale jobs, duplicates or unverified leads. Number rows and use:

| # | 地点 | 岗位 | 为什么值得看 | 还需确认 |
|---|---|---|---|---|
| 1 | 城市 | 公司、职位直链、发布日期证据、已披露薪资 | 具体职责对应的简历证据 | 最大差距或尚未核实的门槛 |

Summarize sources checked, individual descriptions read and any access limits. Ask which roles are worth pursuing. On “下一批” or “都不合适”, reuse the candidate profile and search scope, apply explicit feedback, and search for the next 20. Deduplicate by requisition ID, normalized URL and equivalent employer/title/location; retain progress and displayed IDs within the current search. For optional persistence, use a user-approved private location outside this skill directory.

Use role and location keywords only when querying job sources; do not send the resume, contact details or credentials to job boards. Never package candidate files, profiles, search logs, feedback or credentials with the skill. Do not auto-apply, send messages or schedule searches without authorization.
