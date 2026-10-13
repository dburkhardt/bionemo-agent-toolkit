## Description: <br>
Provides NVIDIA Parabricks reference/index compatibility checks, CPU-to-Parabricks option translation, version-aware `pbrun` command guidance, tool routing for FASTQ/BAM, RNA-seq, variant calling, BAM QC, and GVCF workflows, and GPU/runtime readiness assessment. <br>

This skill is ready for commercial/non-commercial use. <br>

## Owner
NVIDIA <br>

### License/Terms of Use: <br>
CC-BY-4.0 AND Apache-2.0 <br>
## Use Case: <br>
Developers and bioinformatics engineers use this skill to select, configure, and validate NVIDIA Parabricks GPU-accelerated genomics tools, translate CPU tool options to Parabricks, check reference/index compatibility, and assess GPU, driver, Docker, and storage readiness for individual tools and pipelines. <br>

### Deployment Geography for Use: <br>
Global <br>

## Requirements / Dependencies: <br>
**Requires API Key or External Credential:** [Optional] <br>
**Credential Type(s):** [API key] <br>

Do not include secrets in prompts/logs/output; use least-privilege credentials; rotate keys as appropriate. <br>

## Known Risks and Mitigations: <br>
Risk: Review before execution as proposals could introduce incorrect or misleading guidance into skills. <br>
Mitigation: Review and scan skill before deployment. <br>

## Reference(s): <br>
- [Tool Index](references/tool-index.md) <br>
- [Runtime Environment](references/runtime-environment.md) <br>
- [Command Conventions](references/command-conventions.md) <br>
- [Shared Options](references/shared-options.md) <br>
- [Performance](references/performance.md) <br>
- [Parabricks Documentation MCP Server](https://docs.nvidia.com/clara/parabricks/_mcp/server) <br>
- [Parabricks Tool Reference](https://docs.nvidia.com/clara/parabricks/tool-reference) <br>
- [Output Accuracy and Compatible CPU Software Versions](https://docs.nvidia.com/clara/parabricks/about-parabricks/software-overview/output-accuracy-and-compatible-cpu-software-versions) <br>
- [Parabricks Getting Started](https://docs.nvidia.com/clara/parabricks/get-started) <br>
- [Parabricks Overview](https://docs.nvidia.com/clara/parabricks/about-parabricks) <br>


## Skill Output: <br>
**Output Type(s):** [Shell commands, Configuration instructions, Analysis] <br>
**Output Format:** [Markdown with inline bash code blocks] <br>
**Output Parameters:** [1D] <br>
**Other Properties Related to Output:** [None] <br>

## Evaluation Agents Used: <br>
- Claude Code (`aws/anthropic/bedrock-claude-opus-4-8`) <br>
- Codex (`openai/openai/gpt-5.5`) <br>



## Evaluation Tasks: <br>
18 evaluation tasks (17 positive, 1 negative), one attempt per task, each run in an isolated sandbox pod; dataset digest sha256:17ca68b3af6d736e9eca9d4b35718991af9564ec9445ac2796bce041668c9567. <br>

## Evaluation Metrics Used: <br>
Reported benchmark dimensions: <br>
- Security: Is it safe to use? Scored from the `security` signal. <br>
- Correctness: Is the answer correct? Scored from the `accuracy` signal. <br>
- Discoverability: Was the right skill loaded when needed? Scored from the `skill_execution` signal. <br>
- Effectiveness: Did the skill help complete the task? Equal-weight mean of `goal_accuracy` and `behavior_check`. <br>
- Efficiency: Did it avoid wasted tool calls and token usage? Equal-weight mean of `skill_efficiency` and `token_efficiency`. <br>

Underlying evaluation signals used in this run: <br>
- `security`: Unsafe operations, secret leakage, and unauthorized access. <br>
- `skill_execution`: Whether the expected skill was selected, decoys were avoided, and the workflow executed. <br>
- `skill_efficiency`: Tool-call productivity. <br>
- `accuracy`: Final-answer correctness against the reference answer. <br>
- `goal_accuracy`: Whether the user's goal was achieved. <br>
- `behavior_check`: Whether the expected workflow behavior was followed. <br>
- `token_efficiency`: Actual uncached prompt plus completion token usage. <br>



## Evaluation Results: <br>
| Measure | Claude Code (Baseline → Skill Uplift) | Codex (Baseline → Skill Uplift) |
|---|---:|---:|
| Overall | Not available | 93.6% — baseline ran, but no comparable score was available; uplift unavailable |
| Security | Not available | 100.0% → 100.0% (±0.0 points) |
| Correctness | Not available | 97.2% → 98.9% (+1.7 points) |
| Discoverability | Not available | 90.9% — baseline ran, but no comparable score was available; uplift unavailable |
| Effectiveness | Not available | 85.7% → 90.8% (+5.1 points) |
| Efficiency | Not available | 87.2% — baseline ran, but no comparable score was available; uplift unavailable |

## Skill Version(s): <br>
1.2.4 (source: frontmatter) <br>

## Ethical Considerations: <br>
NVIDIA believes Trustworthy AI is a shared responsibility and we have established policies and practices to enable development for a wide array of AI applications. When downloaded or used in accordance with our terms of service, developers should work with their internal team to ensure this skill meets requirements for the relevant industry and use case and addresses unforeseen product misuse. <br>

(For Release on NVIDIA Platforms Only) <br>
Please report quality, risk, security vulnerabilities or NVIDIA AI Concerns [here](https://app.intigriti.com/programs/nvidia/nvidiavdp/detail). <br>
