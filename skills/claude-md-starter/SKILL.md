---
name: claude-md-starter
description: Writes or improves a project's CLAUDE.md so Claude Code knows the stack, the exact run and test commands, and the rules to follow. Use when the user starts a new project, asks to set up or improve CLAUDE.md, or keeps correcting Claude about the same things.
---

# CLAUDE.md Starter

CLAUDE.md is the notes file Claude Code reads at the start of every session. A good one saves the user from repeating themselves. Write one that is short, specific and true for this project.

## 1. Look before asking

Read the project first: the package or build files (package.json scripts, pyproject, Gradle, Makefile), the framework, the folder layout, the test command and any existing CLAUDE.md or README. Run nothing destructive.

## 2. Ask at most three questions

Only ask what the files can't tell you, for example:

- What does "done" mean here (tests pass, works on a real phone, deployed)?
- What should Claude never touch (secrets, generated folders, a shared config)?
- What does Claude keep getting wrong?

## 3. Write CLAUDE.md with these sections

```markdown
# <Project name>

<One or two lines: what this is and who it's for.>

## Stack
- <framework, language, key libraries and versions that matter>

## Commands
- Run: `<exact command>`
- Test: `<exact command>`
- Build or deploy: `<exact command>`

## Map
- `<folder>/`: <what lives there>

## Rules
- <do this>
- <never do that>

## Gotchas
- <something that broke before and how it was fixed>

## Done means
- <how to verify a change before calling it finished>
```

## 4. Keep it lean

- Use bullets, not essays. Aim for under about 150 lines.
- Every command must be copy-paste exact and actually work. Test them if it's safe.
- Write rules as instructions ("Run the tests before committing"), not history.
- Never paste secrets, keys or tokens into CLAUDE.md.

## 5. Keep it alive

Tell the user: whenever Claude repeats a mistake, add one line under Rules or Gotchas. That line stops it happening again.

---

Made by [Try It, Build It](https://tryitbuildit.com). Claude Code tips for beginners: https://tryitbuildit.com/guides/claude-code-tips. More tested Claude skills: https://tryitbuildit.com/skills
