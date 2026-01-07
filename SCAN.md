# SCAN.md – Project Audit for Agentic Upgrade

Run this process to migrate legacy projects:

1. Read entire repo structure (tree -L 3)
2. Identify:
   - Existing instructions (.cursor*, CLAUDE.md, etc.)
   - Tech stack & patterns
   - Pain points (duplication, tests missing, etc.)
   - Decisions not documented
   - Risks/blockers

3. Propose:
   - Merge into new AGENTS.md
   - Populate DECISIONS.md, GLOSSARY.md, TASKS.md
   - Create missing memory files
   - Suggest multi-agent roles needed

4. Output plan → implement incrementally
