# AI Development Workflow

This document describes how our team uses AI tools (Claude, Cursor, Copilot) when developing software.

AI is a productivity tool, not an authority. Developers are responsible for understanding all code before it is committed.

---

# Tools

Approved tools:

- Claude Code
- Cursor
- GitHub Copilot

Optional tools:

- ChatGPT
- Gemini CLI

Never paste proprietary code into public models unless the repository is public.

---

# Guiding Principles

1. Never commit code you don't understand.
2. AI output must pass the same quality bar as human code.
3. AI-generated code must go through normal review and testing.
4. Treat AI as a junior developer.

---

# Standard Development Workflow

## 1. Define the Feature

Before coding, create a short implementation plan.

Prompt example:

"Help me create an implementation plan for this feature.  
Break it into small tasks with acceptance criteria."

Output should be saved as:

plan.md

Example:

1. Add API endpoint
2. Add validation
3. Implement database logic
4. Add tests
5. Update documentation

---

## 2. Implementation

Use AI to implement one task at a time.

Rules:

- Only implement ONE task per commit
- Keep commits small
- Ensure tests pass after each task

Prompt example:

"Implement task #2 from plan.md.  
Follow the existing project architecture."

---

## 3. AI Self-Review

Before opening a PR, run an AI review.

Prompt example:

"Review this code for:
- bugs
- performance issues
- security issues
- style violations"

Fix any issues discovered.

---

## 4. Local Checks

Before pushing code:

Run:

npm run lint  
npm run typecheck  
npm run test

AI can help fix failures.

Prompt example:

"Fix lint and test failures without changing functionality."

---

## 5. Pull Request

PR description must include:

- summary of the change
- relevant plan.md tasks
- whether AI was used

Example:

AI usage:  
Claude generated initial implementation of validation logic.

---

## 6. Human Review

Reviewers should focus on:

- architecture
- maintainability
- correctness
- security

Do not rely on AI review alone.

---

# AI Prompting Guidelines

Good prompts:

- include context
- include examples
- specify constraints

Example:

"Write a function following the same style as utils/cache.ts."

Avoid:

- vague prompts
- large multi-feature prompts
- pasting huge codebases

---

# Files Used by AI

The following files are automatically included in AI context:

- README.md
- ARCHITECTURE.md
- CONTRIBUTING.md
- docs/ai-workflow.md

These files define how the project works.

---

# Things AI Should NOT Do

AI should never:

- change infrastructure configs without approval
- introduce new dependencies without explanation
- modify security-sensitive code without review

---

# When NOT to Use AI

Avoid AI when:

- debugging production incidents
- writing security-sensitive code
- performing complex refactors without a plan

---

# Continuous Improvement

If you discover better prompts or workflows:

Add them to:

docs/ai-patterns.md