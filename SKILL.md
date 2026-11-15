---
name: resume-to-roles
description: Find jobs in any profession or industry from a user's resume and target locations. Verify listings, explain fit, and deliver ranked batches of 20 without repeats.
---

# Resume to Roles

## Start with the candidate

1. If a resume is not available for this search, ask for a file or pasted text. Tell the user they can remove contact details. Reuse a resume already provided for this search.
2. In one short intake question, confirm missing target cities/regions or remote scope, preferred employer types (e.g., multinational, listed company, startup, nonprofit), and employer size (e.g., headcount range or small/midsize/large). Ask only for missing fields, accept “不限” or “跳过” separately for type and size, and reuse choices in later batches. If the user requests an immediate search, leave unspecified employer preferences unrestricted. Do not assume locations, industries or job titles.
3. Derive role families, seniority, adjacent titles, local-language synonyms and search terms from the candidate's demonstrated work, skills and stated goals. For example, a design resume may suggest product design and design systems; an operations resume may suggest business operations and program management; an engineering resume may suggest roles by technical specialty and level. Examples are not default tracks. Record unknown constraints without inventing them.

## Find and verify

**Search narrow to wide.** Aim for 20 unseen, dated candidates in each of the first two batches from the last 7 days, expanding to 10 days if needed. Before using older dates, reuse unseen candidates, vary relevant keywords, paginate and search additional appropriate platforms in the same geography. Only when these routes are exhausted or blocked, widen to 15 days and then 20 days if still short. Keep all 7–10-day candidates ahead of wider-window additions, label the widened tier and explain the coverage gap. Apply the same sequence on later batches; do not change the location without user direction.

Search multiple relevant role families on local boards and directly on employers' career sites. Use [source routing and date rules](references/search-sources.md) for employer feeds, Singapore and Bangkok. For mainland China, search BOSS直聘, 猎聘 and LinkedIn first; use [China portal search](references/china-portals.md). Start with the last 7 calendar days including today, in the user's timezone; if fewer than 20 worthwhile candidates are found, expand to 10 days. Try additional role synonyms, in-scope sources and result pages before returning a short batch; stop when available coverage is exhausted or blocked, or two passes yield no relevant new candidates.

Open individual descriptions for promising roles. Record employer, title, location, direct link, source, job ID, posting-date evidence, status and disclosed pay. Treat first publication, refresh dates and hiring status separately. A list card, crawl date or Apply button alone does not establish current availability. Label missing dates, uncertain status and partial descriptions separately.

Use employer type and size to filter only when the user makes them mandatory; otherwise use them to prioritize similarly suitable roles. Categories can overlap. Verify type and size when relevant from employer disclosures or credible company profiles, distinguishing global headcount from local office or team size. Do not infer them from brand recognition. Flag unknowns in “还需确认”; if a mandatory employer condition is unverified, label the role as pending rather than a confirmed match.

Check explicit requirements first: work location, language, work authorization, licenses and other mandatory credentials. Mark each as met, unmet or unknown. Exclude known hard failures from recommendations. Rank using evidence for responsibilities, skills, seniority and domain; distinguish direct matches, transferable experience and gaps. Match the actual work, not just title or tools: a shared SQL keyword does not establish investment-domain or data-engineering fit. Treat preferences differently from mandatory requirements. Do not invent skills or treat a match score as interview odds.

## Output

Finish an initial pass on all priority sources before selecting the 20, even if one source alone already yields 20. Rank the merged pool; carry over unshown candidates. Keep each platform’s date evidence when merging a duplicate, rather than replacing an original date with a newer refresh.

**Delivery gate: 20 distinct candidates is one complete batch.** Fewer than 20 is progress, not a completed batch. If short, continue the same batch without asking the user to choose roles or request the next batch: use unseen leads, vary in-scope keywords, paginate and cover accessible priority sources. Check coverage at each window (7 → 10 → 15 → 20 days); widen only when the earlier window is exhausted or blocked. Keep user hard requirements unchanged.

Fill the batch in this order: (1) recent original postings, (2) verified recent refreshes or updates, (3) after exhausting the date tiers, worthwhile **待核实线索** without a reliable date. Rank by fit within each tier. Pending leads count toward the same 20 if they have a direct job link, employer/title/location evidence and a concrete fit reason, even if the full JD, date or status is unavailable. Label them individually; never represent them as recent or verified. General list pages without a direct job link, known closed/expired roles, duplicates, known hard mismatches and known out-of-window postings with no recent activity do not count. Dates must be labeled 首发, 刷新/更新 or 日期待核实, separately from JD and hiring status.

Only after accessible search routes and time tiers are exhausted, blocked, or two expanded passes produce no new eligible leads may you stop short. Label the result **同批未满：N/20**, report what you tried and what would unlock more results, and keep the batch open rather than asking for “下一批”. For completed batches, report 20 with the split between dated candidates and date-unverified leads. Use:

| # | 地点 | 岗位 | 为什么值得看 | 还需确认 |
|---|---|---|---|---|
| 1 | 城市 | 公司、职位直链、发布日期证据、已披露薪资 | 具体职责对应的简历证据 | 最大差距或尚未核实的门槛 |

Summarize sources checked, unique leads, individual descriptions actually read, verified matches and access limits. Track summary-only, blocked and closed separately; blocked does not mean closed or zero results. Ask which roles are worth pursuing. On “下一批” or “都不合适”, reuse the candidate profile and search scope, apply explicit feedback, and search for the next 20. Keep a session ledger of source/query/city, last completed page or cursor, access status, candidate identities, and shown IDs (including unverified leads). Reuse unseen eligible candidates before fetching more pages. Deduplicate by employer-scoped requisition ID, normalized URL and equivalent employer/title/location; preserve separate requisitions when evidence shows they differ. Recruiter listings can be candidate duplicates even when boards format the title differently; compare agency, contract duration, location and public reference, and flag uncertainty if the end employer is unknown. When a shown lead is verified later, report it as an update rather than counting it again. For optional persistence, use a user-approved private location outside this skill directory.

Use role and location keywords only when querying job sources; do not send the resume, contact details or credentials to job boards. Never package candidate files, profiles, search logs, feedback or credentials with the skill. Do not auto-apply, send messages or schedule searches without authorization.
