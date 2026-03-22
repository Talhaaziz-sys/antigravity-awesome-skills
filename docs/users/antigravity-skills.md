# Antigravity Skills

If you are using **Antigravity** and want an installable skill library, this repository provides a large collection of `SKILL.md` playbooks that work with the Antigravity IDE's global and workspace skill paths, along with several skills built specifically for Antigravity sessions.

Antigravity Awesome Skills supports Antigravity through the `~/.gemini/antigravity/skills/` global path and the `.agent/skills/` workspace path. It includes skills designed to improve planning, UI engineering, skill orchestration, and workflow execution inside Antigravity.

## Why use this repo for Antigravity

- It installs directly into the expected Antigravity skill paths.
- It includes skills built specifically *for* Antigravity (listed below).
- It ships with bundles and workflows so you have a guided starting point instead of browsing 1,306+ skills cold.
- It covers the full engineering cycle: planning, UI, backend, testing, security, infrastructure, and product work.

## Install Antigravity Skills

```bash
npx antigravity-awesome-skills --antigravity
```

### Verify the install

```bash
test -d ~/.gemini/antigravity/skills && echo "Skills installed in ~/.gemini/antigravity/skills"
```

Use `--path .agent/skills` for a workspace-scoped install instead of global:

```bash
npx antigravity-awesome-skills --path .agent/skills
```

## Skills Built for Antigravity

These skills were designed specifically to work with or extend Antigravity:

### [`antigravity-workflows`](../../skills/antigravity-workflows/)

Orchestrates multiple Antigravity skills through guided workflows. Covers common multi-phase goals:

- Ship a SaaS MVP
- Run a web security audit
- Build an AI agent system
- Execute browser QA automation
- Design a DDD core domain

Use this skill when the user wants a best-practice execution sequence without manually selecting each skill.

### [`antigravity-design-expert`](../../skills/antigravity-design-expert/)

Core UI/UX engineering skill for building highly interactive, spatial, and weightless web interfaces. Specializes in:

- Glassmorphism and floating card layouts
- GSAP + ScrollTrigger scroll-linked animations
- Isometric CSS 3D transforms
- React Three Fiber (R3F) 3D elements
- Staggered entrance animations and parallax effects

Use this skill when building premium-feeling, motion-rich UIs.

### [`antigravity-skill-orchestrator`](../../skills/antigravity-skill-orchestrator/)

A meta-skill that evaluates task complexity, discovers the right skills from the local environment or the master catalog, and tracks successful skill combinations using `@agent-memory-mcp`. It enforces strict guardrails to avoid using specialized skills on simple tasks.

Use this skill when facing a complex, multi-domain problem and you want the agent to find and coordinate the right skills automatically.

### [`analyze-project`](../../skills/analyze-project/)

Forensic root cause analyzer for Antigravity sessions. Classifies scope deltas, rework patterns, root causes, and hotspots, and auto-improves prompts and project health scores. Originally designed to analyze Antigravity session history for quality and efficiency improvements.

Use this skill after a difficult or overscoped session to diagnose what went wrong and how to improve.

### [`blockrun`](../../skills/blockrun/)

Designed to work with both Claude Code and Antigravity. Provides block-execution patterns for running structured code segments within an Antigravity environment.

## Example Antigravity Prompts

```text
Use @antigravity-workflows to run the "Ship a SaaS MVP" workflow for my project.
```

```text
Use @antigravity-design-expert to build a floating glassmorphism card grid with staggered entrance animations.
```

```text
Use @antigravity-skill-orchestrator to find the right skills for building a multi-tenant auth system.
```

```text
Use @analyze-project to review this session and identify the root cause of the scope creep.
```

## What to do next

- Start with [`bundles.md`](bundles.md) if you want a role-based shortlist (for example: Full-Stack Developer, Security Engineer).
- Use [`workflows.md`](workflows.md) for step-by-step execution playbooks starting from `antigravity-workflows`.
- Read [`usage.md`](usage.md) for more prompt examples and invocation patterns.
- Go back to the main [`README.md`](../../README.md) for the full installation matrix and tool comparison.
