# local-ai-systems-studio

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-111827?style=flat-square)](./SKILL.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](./LICENSE)
[![Public Repo](https://img.shields.io/badge/Repo-Public-2563eb?style=flat-square)](https://github.com/however-yir/codex-skill-local-ai-systems-studio)
[![Last Commit](https://img.shields.io/github/last-commit/however-yir/codex-skill-local-ai-systems-studio?style=flat-square)](https://github.com/however-yir/codex-skill-local-ai-systems-studio/commits/main)

> Plan, compare, deploy, and structure local AI systems without overengineering them.

中文简介：这是一个面向本地 AI 系统规划的 Codex skill，适合把问题定义、模型与工具选择、本地部署路径、工作流设计和执行计划串成一条完整链路。

A Codex skill for turning local AI ideas, deployment questions, and workflow problems into practical end-to-end plans.

Use this when the main uncertainty is still about local stack choice, deployment path, model format, or hardware fit. If those decisions are already made and the remaining work is deeper workflow orchestration, `ai-agent-workflow` is usually the better fit. If the main task becomes creating, rewriting, benchmarking, or optimizing a skill artifact itself, `skill-creator` is usually the better fit.

## What This Skill Does

This skill helps scope a local AI problem, compare tools and models, recommend a realistic deployment path, and convert the decision into a concrete plan.

## Best For

- local LLM selection
- LM Studio versus Ollama versus MLX decisions
- GGUF and deployment tradeoffs
- practical AI workflow design
- issue-to-plan conversion for local AI systems
- choosing the smallest stack that still gets the job done

## Inputs

Typical inputs:
- the task to solve
- device and hardware constraints
- preferred local tools or runtimes
- latency, privacy, or quality expectations
- current workflow draft or problem report

## Outputs

Typical outputs:
- clarified job-to-be-done
- model or tool comparison
- deployment recommendation
- workflow architecture outline
- phased implementation plan
- risk notes and next actions

## Non-goals

This skill is not aimed at:
- purely cloud AI architecture
- creating or benchmarking a skill artifact itself
- one-off content writing
- specialized training pipelines
- deep backend code changes unrelated to local AI workflows

## Example Prompts

- `Should I use LM Studio, Ollama, or MLX for this local AI workflow?`
- `Help me turn this local AI issue into an execution plan.`
- `Design a practical local workflow for PDF summary and task extraction.`
- `Compare model and tool options for a Mac-first local setup.`

## Routing Notes

- Use this skill when the first hard question is still stack choice, deployment path, model format, or hardware fit.
- If the stack is already mostly chosen and the remaining work is workflow orchestration, route to `ai-agent-workflow`.
- If the task becomes "create this as a skill", "improve this skill", or "benchmark this skill", route to `skill-creator`.

## Repository Structure

```text
.
├── .gitignore
├── LICENSE
├── README.md
├── SKILL.md
├── assets/
│   └── .gitkeep
├── examples/
│   └── showcase.md
├── references/
│   └── checklist.md
└── scripts/
    └── .gitkeep
```

## Showcase Examples

See [examples/showcase.md](./examples/showcase.md) for three stronger examples covering stack selection, workflow design, and local issue triage.

## Included Files

- [SKILL.md](./SKILL.md): trigger logic, workflow, examples, and pairing guidance
- [examples/showcase.md](./examples/showcase.md): public-facing showcase examples
- [references/checklist.md](./references/checklist.md): end-to-end planning checklist
- [LICENSE](./LICENSE): MIT license for future standalone publication

## Pair Well With

- `ai-agent-workflow`
- `mcp-server-builder`
- `prompt-optimizer`
- `deep-research`
- `skill-creator`

## License

Released under the MIT License. See [LICENSE](./LICENSE).

## Notes

This skill is intentionally practical. It prefers a well-chosen simple local stack over a flashy but fragile workflow.
