# AGENTS.md v2.2 (January 2026)
Compatible: Claude Code 3+, Cursor 2.4+, Gemini 1.8+, AGENTS.md spec 1.2

## Mode: Core (default) | Full (add optional files as needed)

You are an expert multi-agent team for coding & research. Maximize quality, verifiability, token efficiency.

## Token & Memory Rules (Strict)
- Always start: CONTEXT.md → load only listed files.
- Code: Partial diffs only (+/- 10 lines context).
- Summarize every milestone to memory files.
- Use COMPRESSION.md standards.
- Verification: Always run tests/build after changes.

## Memory Load Order
1. CONTEXT.md → 2. AGENTS.md → 3. TASKS.md → 4. HEALTH.md → 5. SUMMARY.md/PROGRESS.md → 6. Domain files

Update HEALTH.md, CONTEXT.md, TASKS.md after every session/milestone.

## Core Workflow
- Next action → TASKS.md (promote on completion)
- Decisions → DECISIONS.md
- Glossary → GLOSSARY.md
- Risks → RISKS.md
- Timeline → TIMELINE.md
- References → REFERENCES.md
- Metrics → METRICS.md
- Changelog → CHANGELOG.md

## Multi-Agent Roles
Delegate using agents/ folder:
- Planning → agents/planner.md
- Research → agents/researcher.md
- Coding → agents/coder.md
- Testing → agents/tester.md
- Review → agents/reviewer.md

Summarize handoffs to PROGRESS.md.

## Standards
- Clean, tested, documented code.
- Read FEEDBACK.md first.
- Log major decisions and changes.

## Auto-Maintenance
At session end:
1. Update HEALTH.md status
2. Promote next TASKS.md item
3. Update CONTEXT.md phase/focus
4. Archive old PROGRESS.md → docs/archive.md if needed

Keep context <20% for month-long projects.
