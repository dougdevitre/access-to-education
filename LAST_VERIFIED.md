# Data Verification Log

**Purpose:** Track when specific data points, numbers, and facts were last verified. When a data point is marked "approximate" or "varies," this log records the source and verification date so maintainers know what needs refreshing.

**Review cycle:** Quarterly review of all "High" volatility items. Annual review of "Medium" items. "Low" items reviewed on the standard 5-year content review cycle.

---

## Where facts are tracked

Every phone number, dollar figure, deadline and program-status claim that has been verified on its primary source lives in **`facts/ledger.json`**, one entry per fact with the source URL, the verification date, the recheck interval and the files that state it. `scripts/check-facts.mjs` runs in CI (`Validate Content` → `Fact ledger`) and fails when a fact is past its recheck date, a listed file is missing, or the value no longer appears in any listed file. To refresh a fact: re-check it on the source, then update `verified_on` (and the value and files if they changed). Never add an entry you did not verify that day, and never back-date one.

The table below holds the data points **not yet in the ledger**: each was recorded on the date shown, but was not re-checked on a primary source on the day the ledger was built, so CI does not yet vouch for it. Move a row into `facts/ledger.json` once you have confirmed it on the source.

## Awaiting verification

| File | Data Point | Value | Source | Last Verified | Volatility |
| ------ | ----------- | ------- | -------- | -------------- | ------------ |
| mo-districts-regions.md | Total public school districts | ~518 | DESE MCDS | 2025-10 | Medium |
| mo-districts-regions.md | Total student enrollment | ~880,000 | DESE MCDS | 2025-10 | High |
| mo-districts-regions.md | Total certified staff | ~69,000 | DESE Core Data | 2025-10 | High |
| mo-districts-regions.md | Student race/ethnicity %s | See file | DESE MCDS | 2025-10 | Medium |
| mo-districts-regions.md | FRPM eligibility % | ~45-50% | DESE MCDS | 2025-10 | High |
| educator-workforce.md | PSRS contribution rate | ~14.5% | PSRS.org | 2026-10 | Medium |
| educator-workforce.md | PEERS contribution rate | ~6.86% | PSRS.org | 2026-10 | Medium |
| educator-workforce.md | NBCT supplement amount | No statewide supplement confirmed; district incentives only (RSMo 168.345 does not exist) | DESE NBC district incentives | 2026-10 | Low |
| students.md | Minimum graduation credits | 24 | DESE | 2025-08 | Low |
| students.md | Access Missouri amounts | $300-$2,850/yr | MDHEWD | 2025-01 | High |
| teachers.md | Non-renewal deadline | April 15 | RSMo 168.126 | 2026-10 | Low |
| teachers.md | Probationary period | 5 years | RSMo 168.104 | 2025-08 | Low |
| specialists.md | Evaluation timeline | 60 calendar days | IDEA §300.301 | 2025-08 | Low |
| specialists.md | IEP annual review | Every 365 days | IDEA §300.324 | 2025-08 | Low |
| assessments.md | EOC required subjects | Eng II, Alg I, Bio, Am Gov | DESE | 2025-08 | Medium |
| facilities-operations.md | Bond approval requirement | 4/7 at general municipal, primary or general elections; 2/3 at other elections | Mo. Const. art. VI §26(b) | 2026-10 | Low |
| rural-education.md | % districts on 4-day week | ~25% | DESE/media reports | 2025-10 | Medium |
| ai-in-education/ | DESE AI guidance version | 1.0 (2025-26) | DESE | 2025-07 | High |
| ai-in-education/ | SB 68 signed | July 9, 2025 | Missouri Legislature | 2026-10 | Low |
| ai-in-education/ | States with AI guidance | 31+ | aiforeducation.io | 2026-01 | High |
| school-staff.md | Mandated reporter penalty | Class A misdemeanor | RSMo 210.165 | 2026-10 | Low |

---

## Statute Verification

All RSMo citations in this skill were verified against the Missouri Revised Statutes as of **2025-08**. Missouri legislative sessions may enact changes annually (session: January-May). After each legislative session, review:
1. Education bills signed by the Governor
2. DESE administrative memos reflecting new laws
3. MSBA legislative summary

**Next legislative review due:** June 2026 (after 2026 session concludes)

---

## Federal Law Verification

Federal citations (IDEA, ESSA, Title IX, FERPA, ADA, etc.) were verified as of **2025-08**. Federal regulatory changes occur through the Federal Register. Monitor:
1. U.S. Department of Education Dear Colleague Letters
2. Federal Register notices affecting education
3. Supreme Court decisions affecting education law

---

## Content Review Dates

| File | Last Full Content Review |
| ------ | ------------------------ |
| SKILL.md | 2026-03 |
| All references/*.md | 2026-03 (initial creation) |
| All references/ai-in-education/*.md | 2026-03 (initial creation) |
| All references/curriculum-instruction/*.md | 2026-03 (initial creation) |
| templates/*.md | 2026-03 (initial creation) |
