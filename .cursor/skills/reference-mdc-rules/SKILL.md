---
name: reference-mdc-rules
description: Ensures the agent reads and applies all .mdc rules in .cursor/rules/ for every prompt. Use for every response so that all Cursor rule requirements are followed by all agents.
---

# Reference All .mdc Rules for Every Prompt

## Instructions

For **every** prompt (in any mode: Agent, Plan, Debug, Ask):

1. **Load all rules**: Read every file in `.cursor/rules/` matching `*.mdc`.
2. **Apply every rule**: Follow each rule’s instructions in addition to answering the user. Do not skip rules; treat all .mdc rules as required for every response.
3. **Order**: Apply rules in the order they are needed (e.g. state model at start of response; append to AIprompts.md after the response).

## Finding Rules

- **Location**: `.cursor/rules/*.mdc`
- **Discovery**: List `.cursor/rules/` or use glob `**/*.mdc` under `.cursor/rules/` to get the current set. New or renamed .mdc files must be included.

## Summary of Current Rules (this project)

| Rule file | Purpose |
|-----------|--------|
| `state-model-before-response.mdc` | At start of each response, state which AI model is being used (one short line). |
| `append-prompts-to-aiprompts.mdc` | After each response, append to `AIprompts.md`: separator, Model, Mode, Prompt, then separator again. Preserve existing content. |

When new .mdc rules are added to `.cursor/rules/`, include them in this workflow; the table above is a snapshot for convenience, not an exhaustive contract.
