# How the workflow fits together

## 1. Architect: define the work

The Architect translates a goal into scoped tasks and dependencies. Requirements and acceptance criteria give implementation and review a shared target.

## 2. Builders: implement scoped changes

Developer tasks use separate Git worktrees. Independent tasks can run in parallel within the configured capacity; dependent tasks wait for their prerequisites. Worktrees keep working directories separate, while dependency and merge handling still matter when changes come together.

## 3. Reviewers: assess the proposed work

Independent reviewers use a different model/provider from implementation to inspect changes against the requirements and available evidence. Findings may require corrections before the task advances. A review is an additional assessment, not a guarantee that every defect will be found.

## 4. Checks and delivery: inspect the evidence

Project checks can include tests, type checking, linting or builds, depending on the repository and configuration. Completion reports make the proposed changes, reviewer findings and check results easier to inspect.

Always distinguish a check that passed from one that failed, was skipped or could not run. Passing checks establish only what those commands and criteria actually cover.

## Approval and automation

Project settings control how work advances and where human approval is required. Review the chosen settings before starting. Use the available pause/stop controls when you need to inspect or interrupt a run.

## Example evaluation

For a validation change, define the expected accepted/rejected input, implement the rule and tests, review the diff with another model, then inspect test and build results. The useful output is a traceable change with evidence you can evaluate.

## What Coterie coordinates

Coterie coordinates supported official coding CLIs and their existing provider access. It is not an AI-model tournament, an API service for arbitrary multi-model inference, or a promise of perfect code.
