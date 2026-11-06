# Working with Codex

This repository is both a curriculum and a portfolio workspace. Use Codex as a **mentor/reviewer by default**, not as a substitute for practicing.

## Initial setup
1. Clone the repository and open its root as the Codex workspace.
2. Codex reads root `AGENTS.md` as repository instructions when it supports this convention. In any other environment, explicitly instruct the assistant to read it.
3. Keep the solutions and the progress log committed to Git. Pull remote changes before starting a new session.

## Daily workflow
1. **Start:** Ask Codex to read `AGENTS.md`, `PROGRESS.md` and `TASKS.md`. Request the current task's exact requirements, no solution.
2. **Study:** Explain the theory back in your own words. Ask for hints only when blocked.
3. **Implement:** Create a task-specific source file (e.g. `week-01/JS-001.js`). Write the solution yourself.
4. **Review:** Ask Codex to inspect code and run safe tests. Request feedback and a /10 score, **without editing the solution**.
5. **Fix:** Make corrections yourself, retest and re-request review.
6. **Record:** Once criteria pass, explicitly ask Codex to update `PROGRESS.md` with evidence, score and commit reference.
7. **Commit/push:** Keep one clear Git history per task. Suggested commit format: `feat(js-001): implement counter`.

## Example prompts

**Start learning**
> Read AGENTS.md, TASKS.md and PROGRESS.md. Identify my next unfinished task. Teach the prerequisites in Ukrainian and restate its exact acceptance criteria. Do not write the solution.

**Ask for a hint**
> I am stuck on JS-001. Give me only hint level 1. Do not edit my files or reveal code.

**Review**
> Review week-01/JS-001.js against JS-001 in TASKS.md. Run appropriate tests if possible. Give strict /10 feedback and edge cases, but do not change my solution or update progress yet.

**Record the result**
> The task has passed review. Update only the relevant rows in PROGRESS.md using the actual code/test evidence and current commit. If evidence is insufficient, do not mark DONE.

**Weekly interview**
> Read my completed tasks and review log. Conduct a week-1 mock interview without hints. Ask questions one at a time, score my responses, and prepare a checkpoint entry for PROGRESS.md. Do not mark VERIFIED without an independent exercise.

**When implementation help is really needed**
> Switch to implementation mode for this explicitly requested bug only. Explain the change and run tests. Do not mark other tasks completed.

## Status meanings
- `TODO`: not started.
- `IN_PROGRESS`: code in progress, not passed.
- `NEEDS_FIXES`: reviewed with important gaps.
- `DONE`: task acceptance criteria passed, evidence logged.
- `VERIFIED`: skill independently retested without hints.

## Anti-hallucination checklist
- Is every completion claim supported by a file/commit/test?
- Did Codex actually run the tests it describes?
- Is the task specification identical to `TASKS.md`?
- Is the next task consistent with `PROGRESS.md`?
- Did Codex give guidance instead of doing the student's assignment by default?

## Suggested weekly cadence
Mon–Thu: JS/TS/React theory and tasks (1.5 h/day); Fri: interview recap (1 h); Sat: project (4 h); Sun: review/mock (3 h). Adjust to real life, never mark work done just because a date passed.
