# Skill Benchmark: parabricks

> **Overall verdict: NEUTRAL — One or more dimensions remain below PASS**

Live evaluation did not show a material gain or regression. Collect more evidence or improve the skill before making a publication decision.

## Evaluation Metadata

- Skill: `parabricks`
- Evaluation date: 2026-10-13
- Evaluator version: `1.5.6`
- Agents: Claude Code (`aws/anthropic/bedrock-claude-opus-4-8`), Codex (`openai/openai/gpt-5.5`)
- Tasks: 18 evaluation tasks (17 positive, 1 negative)
- Dataset digest: `sha256:17ca68b3af6d736e9eca9d4b35718991af9564ec9445ac2796bce041668c9567` (skill-evaluator-dataset-snapshot/1)
- Attempts per task: 1
- Environment: `k8s-sandbox`
- Tier 2 evidence: required for publication
- Tier 3 evidence: required for publication

Each task attempt ran in its own isolated sandbox pod.

## What This Report Answers

The three-tier evaluation checks whether the skill:

- is safe to use;
- produces correct answers;
- is discovered and activated when needed;
- helps the agent complete the user's goal and expected workflow; and
- avoids wasted skill and tool usage.

## Results at a Glance

| Measure | Claude Code (Baseline → Skill Uplift) | Codex (Baseline → Skill Uplift) |
|---|---:|---:|
| Overall | Not available | 93.6% — baseline ran, but no comparable score was available; uplift unavailable |
| Security | Not available | 100.0% → 100.0% (±0.0 points) |
| Correctness | Not available | 97.2% → 98.9% (+1.7 points) |
| Discoverability | Not available | 90.9% — baseline ran, but no comparable score was available; uplift unavailable |
| Effectiveness | Not available | 85.7% → 90.8% (+5.1 points) |
| Efficiency | Not available | 87.2% — baseline ran, but no comparable score was available; uplift unavailable |

**How to read this table:** baseline is the same task attempted without the target skill. Scores are rounded to one decimal; threshold-adjacent values use additional precision so their displayed band matches the verdict. Uplift is derived from those displayed scores and shown in percentage points.

Example: `47.0% → 92.0% (+45.0 points)` means the skill-assisted run scored 92.0%, 45.0 percentage points above its 47.0% no-skill baseline.

A partial dimension was calculated from only the available configured signals; review the detailed report before relying on it.

## Token Usage

Actual Tier 3 execution usage is reported for every observed agent/case pair and both conditions.

| Agent | Dataset case | With skill | Without skill | Delta | Change | Coverage |
|---|---|---:|---:|---:|---:|---|
| claude-code | All cases | 4,632,174 | 6,282,412 | -1,650,238 | -26.27% | skill 18/18; base 18/18 |
| claude-code | parabricks-001 | 180,273 | 126,697 | +53,576 | +42.29% | skill 1/1; base 1/1 |
| claude-code | parabricks-002 | 118,303 | 32,299 | +86,004 | +266.27% | skill 1/1; base 1/1 |
| claude-code | parabricks-003 | 110,686 | 194,335 | -83,649 | -43.04% | skill 1/1; base 1/1 |
| claude-code | parabricks-004 | 60,303 | 90,709 | -30,406 | -33.52% | skill 1/1; base 1/1 |
| claude-code | parabricks-005 | 118,745 | 34,737 | +84,008 | +241.84% | skill 1/1; base 1/1 |
| claude-code | parabricks-006 | 117,971 | 33,485 | +84,486 | +252.31% | skill 1/1; base 1/1 |
| claude-code | parabricks-007 | 106,319 | 153,277 | -46,958 | -30.64% | skill 1/1; base 1/1 |
| claude-code | parabricks-008 | 158,647 | 32,681 | +125,966 | +385.44% | skill 1/1; base 1/1 |
| claude-code | parabricks-009 | 343,105 | 40,740 | +302,365 | +742.18% | skill 1/1; base 1/1 |
| claude-code | parabricks-010 | 258,857 | 313,527 | -54,670 | -17.44% | skill 1/1; base 1/1 |
| claude-code | parabricks-011 | 166,385 | 40,008 | +126,377 | +315.88% | skill 1/1; base 1/1 |
| claude-code | parabricks-012 | 109,069 | 499,031 | -389,962 | -78.14% | skill 1/1; base 1/1 |
| claude-code | parabricks-013 | 292,103 | 1,517,085 | -1,224,982 | -80.75% | skill 1/1; base 1/1 |
| claude-code | parabricks-014 | 117,563 | 46,682 | +70,881 | +151.84% | skill 1/1; base 1/1 |
| claude-code | parabricks-015 | 167,914 | 38,792 | +129,122 | +332.86% | skill 1/1; base 1/1 |
| claude-code | parabricks-016 | 1,211,920 | 1,262,943 | -51,023 | -4.04% | skill 1/1; base 1/1 |
| claude-code | parabricks-017 | 809,597 | 1,304,656 | -495,059 | -37.95% | skill 1/1; base 1/1 |
| claude-code | parabricks-018 | 184,414 | 520,728 | -336,314 | -64.59% | skill 1/1; base 1/1 |
| codex | All cases | 2,189,290 | 1,106,159 | +1,083,131 | +97.92% | skill 18/18; base 18/18 |
| codex | parabricks-001 | 71,759 | 177,435 | -105,676 | -59.56% | skill 1/1; base 1/1 |
| codex | parabricks-002 | 50,974 | 26,452 | +24,522 | +92.70% | skill 1/1; base 1/1 |
| codex | parabricks-003 | 50,851 | 56,414 | -5,563 | -9.86% | skill 1/1; base 1/1 |
| codex | parabricks-004 | 24,666 | 14,286 | +10,380 | +72.66% | skill 1/1; base 1/1 |
| codex | parabricks-005 | 115,804 | 31,668 | +84,136 | +265.68% | skill 1/1; base 1/1 |
| codex | parabricks-006 | 50,649 | 44,325 | +6,324 | +14.27% | skill 1/1; base 1/1 |
| codex | parabricks-007 | 50,139 | 28,542 | +21,597 | +75.67% | skill 1/1; base 1/1 |
| codex | parabricks-008 | 94,941 | 32,755 | +62,186 | +189.85% | skill 1/1; base 1/1 |
| codex | parabricks-009 | 98,393 | 51,465 | +46,928 | +91.18% | skill 1/1; base 1/1 |
| codex | parabricks-010 | 125,876 | 37,750 | +88,126 | +233.45% | skill 1/1; base 1/1 |
| codex | parabricks-011 | 95,106 | 25,405 | +69,701 | +274.36% | skill 1/1; base 1/1 |
| codex | parabricks-012 | 118,176 | 30,814 | +87,362 | +283.51% | skill 1/1; base 1/1 |
| codex | parabricks-013 | 127,797 | 28,498 | +99,299 | +348.44% | skill 1/1; base 1/1 |
| codex | parabricks-014 | 51,150 | 21,152 | +29,998 | +141.82% | skill 1/1; base 1/1 |
| codex | parabricks-015 | 96,201 | 30,278 | +65,923 | +217.73% | skill 1/1; base 1/1 |
| codex | parabricks-016 | 677,480 | 213,646 | +463,834 | +217.10% | skill 1/1; base 1/1 |
| codex | parabricks-017 | 199,533 | 186,043 | +13,490 | +7.25% | skill 1/1; base 1/1 |
| codex | parabricks-018 | 89,795 | 69,231 | +20,564 | +29.70% | skill 1/1; base 1/1 |
| ALL AGENTS | Dataset aggregate | 6,821,464 | 7,388,571 | -567,107 | -7.68% | skill 36/36; base 36/36 |

Prompt tokens include cached reads, so total tokens are `prompt + completion` (cached is not added twice). The Efficiency score uses `(prompt - cached) + completion`. N/A means the relevant trajectory counters were not available; coverage is never estimated.

## Tier Status

| Tier | Purpose | Status | Evidence |
|---|---|---|---|
| Tier 1 | Static validation | **PASSED WITH OBSERVATIONS** | 11 validator(s); 59 finding(s) |
| Tier 2 | Semantic deduplication | **PASSED WITH OBSERVATIONS** | 2 validator(s); 1 finding(s) |
| Tier 3 | Live agent evaluation | **NEUTRAL** | 2 agent(s); 18 task(s) |

## Findings and Observations

<details>
<summary>Show detailed findings and successful checks</summary>

- **CRITICAL** CONTENT_DEDUP/llm_cluster_member_limit: A Tier 2 cluster exceeds the LLM member limit. (`skills/bionemo-agent-toolkit/skills/parabricks`)
- **MEDIUM** QUALITY/quality_correctness: No documented scripts in table format (`skills/bionemo-agent-toolkit/skills/parabricks/SKILL.md`)
- **MEDIUM** QUALITY/quality_correctness: Instructions don't mention 'run_script' (`skills/bionemo-agent-toolkit/skills/parabricks/SKILL.md`)
- **MEDIUM** QUALITY/quality_reliability: MCP skill lacks connection/error guidance (`skills/bionemo-agent-toolkit/skills/parabricks/SKILL.md`)
- **MEDIUM** QUALITY/quality_efficiency: Deeply nested references in command-conventions.md (`skills/bionemo-agent-toolkit/skills/parabricks/SKILL.md`)
- 55 additional finding(s) are available in the full evaluation artifacts.

</details>

## Scoring Methodology

<details>
<summary>Show dimension definitions, source signals, and thresholds</summary>

| Dimension | Question | Scored signals |
|---|---|---|
| Security | Is it safe to use? | `security` (100%) |
| Correctness | Is the answer correct? | `accuracy` (100%) |
| Discoverability | Was the right skill loaded when needed? | `skill_execution` (100%) |
| Effectiveness | Did the skill help complete the task? | `goal_accuracy` (50%) + `behavior_check` (50%) |
| Efficiency | Did it avoid wasted tool calls and token usage? | `skill_efficiency` (50%) + `token_efficiency` (50%) |

- Dimension bands: PASS at 50% or above; NEUTRAL from 40% to below 50%; FAIL below 40%.
- Overall Tier 3 lift: PASS at +5 points or more; FAIL at -10 points or less; values between those bands are NEUTRAL.
- Overall verdict: PASS only when every configured dimension passes for at least one supported agent. Lift is reported as diagnostic evidence and does not override this gate.
- The 50% attempt pass threshold is a separate per-task gate; it is not the dimension pass threshold.
- Effectiveness is the equal-weight mean of goal completion (`goal_accuracy`) and expected workflow adherence (`behavior_check`).
- Efficiency is 50% tool-call productivity (the backward-compatible `skill_efficiency` wire id) and 50% `token_efficiency`. Positive-case skill routing is scored under Discoverability, not Efficiency; a negative case without a routing target is N/A. N/A sources are omitted, remaining weights are renormalized, and the dimension is marked partial.

Signals present in this run:

- `security` (Security): unsafe operations, secret leakage, and unauthorized access.
- `skill_execution` (Skill Execution): whether the expected skill was selected, decoys were avoided, and the workflow executed.
- `skill_efficiency` (Tool Productivity): tool-call productivity (legacy wire id; routing is scored under Discoverability).
- `accuracy` (Accuracy): final-answer correctness against the reference answer.
- `goal_accuracy` (Goal Accuracy): whether the user's goal was achieved.
- `behavior_check` (Behavior Check): whether the expected workflow behavior was followed.
- `token_efficiency` (Token Efficiency): actual uncached prompt plus completion usage (50% of Efficiency).

</details>

## Freshness

Regenerate this benchmark when the skill, evaluation dataset, target agent/model, evaluator version, environment, or scoring policy changes.
