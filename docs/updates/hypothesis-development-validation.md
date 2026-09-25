# v0.2 candidate validation — release gate not met

Date: 2026-09-24. Baseline: `1af668787d62a285eef46b56013372aeca3bf610`.

**Decision: retain the candidate; do not merge.** All prescribed writing runs and comparisons were completed. The candidate passed the tested factual, evidence and editing-permission conditions, with no confirmed material regression, but did not meet the predeclared improvement threshold.

## Actual execution and results

- 88/88 task-version runs:44 baseline and44 candidate;98 completed writer turns. All10 permission cases used two genuine sequential turns, with approval supplied only after the first response.
- 44/44 fresh-context blinded pair grades, plus3 reversed-position reviews. Original and reviewed judgments agreed:42 ties and2 individual candidate preferences (D02 repetition4 and R01 repetition3).
- Candidate hard conditions:44/44 passed. Confirmed material regression cases:0.
- Theory cases meeting the required majority-improvement criterion:0/6; the release gate required at least4/6, with improvement in both languages. Individual preferences did not constitute case-level improvement.
- All six regression cases showed no confirmed material decline in this limited evaluation. This does not establish global equivalence or statistical non-inferiority.
- Three earlier interrupted attempts were preserved and their same slots retried after resources became available. They were not counted as additional successful repetitions or hidden failures. No prescribed task remains unrun.

| 案例 | 检查重点 | 成对比较 | 偏向新版 | 平局 | 新版硬性检查 |
|---|---|---:|---:|---:|---:|
| D01 | 综述前提与假设推进 | 3 | 0 | 3 | 3/3 |
| D02 | 期待基线与相邻关系 | 5 | 1 | 4 | 5/5 |
| D03 | 条件与线索水平的对应比较 | 5 | 0 | 5 | 5/5 |
| D04 | 机制、干预与效应差异 | 3 | 0 | 3 | 3/3 |
| D05 | 并行路径与段落承接 | 5 | 0 | 5 | 5/5 |
| D06 | 行文、心理与检验顺序 | 3 | 0 | 3 | 3/3 |
| R01 | 引言叙事 | 3 | 1 | 2 | 3/3 |
| R02 | 标题与摘要 | 3 | 0 | 3 | 3/3 |
| R03 | 统计报告 | 3 | 0 | 3 | 3/3 |
| R04 | 方法叙述 | 3 | 0 | 3 | 3/3 |
| R05 | 讨论与局限 | 3 | 0 | 3 | 3/3 |
| R06 | 段落审批与获批范围 | 5 | 0 | 5 | 5/5 |

## Separate diagnostic and technical checks

One runtime smoke check and eight fresh-context diagnostic calls were completed outside the88 formal runs. The diagnostics covered30 baseline outputs. A methods output was146–147 words against a requested150–210; its original hard-fail label remains preserved as a length-compliance issue. Blind comparison and reversed review kept this separate from factual and permission errors. No original grade was erased.

Independent metadata and arithmetic review confirmed the 88 writing runs, 98 turns and 47 separate grader sessions, including the final release-gate calculation. Independent harness review completed14 synthetic gate checks; these are technical checks, not additional writing tests. Skill validation, YAML/name consistency, relative links, public inventory, protected-file comparison and frozen-payload checks passed. Original eight guides, original12 scenarios, source index and visible paragraph approval section retain exact content at their new paths. Publication-history and checksum issues found during static review were corrected.

## Control conditions and limits

Writers and automatic graders used `gpt-6-astra` with `high` reasoning. The precise model snapshot, temperature and seed were not exposed. Writers used fresh isolated contexts, the same controlled inputs/settings and the designated skill copy. Read events, command argument paths, visible runtime contexts and manifests were audited. Read-only permissions are not host-wide read confinement; these checks establish observed behavior only. Copied scenario files were not read by writers.

All88 writers read the assigned skill entry. New09 was read in24/24 candidate theory tasks,0/15 R01–R05 regression tasks and5/5 R06 permission tasks. The last category is reported descriptively, not treated as a writing failure. The rule editor did not read holdout prompts or raw answers; holdout was unsealed by the independent evaluator only after the candidate freeze and development validation.

Candidate skill payload SHA256: `f37867c371a33361dc0a889ab44e22cdcad39d4e662b529788b9996f1e1d041d`.

These are12 fictional case types with repetitions, not88 different research situations. Model-based grading is not human expert acceptance. Original12 and added15 scenario files were retained and mapped but were not individually executed as27 further model tests. Real-manuscript acceptance and client installation tests were not performed.

## Publication and distribution

The repository was renamed to `ld_skill` and remains public. Its main content remains at the baseline. The connector rejected remote branch creation with HTTP403 (`Resource not accessible by integration`); no alternate write interface was used to bypass that rejection. No PR, merge or release was created. Even restored write access would not waive the unmet quality gate for this candidate.

Only generic rules, original generic scenarios and this sanitized summary are packaged. Raw outputs, private records, source manuscripts and the handoff ZIP are excluded. No license or client skill installation was changed. Keep the existing version in use; any later revision needs a new, appropriately separated evaluation before claiming improvement.
