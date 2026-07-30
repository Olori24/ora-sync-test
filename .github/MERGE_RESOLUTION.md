Merge resolution: Jules → foundation/initial

I merged changes from the Jules branch into foundation/initial and resolved conflicts to preserve functionality and keep the newest compatible files.

Conflicts detected and resolution details:

- README.md
  - Conflict: Jules contained an older placeholder README, foundation/initial contains an expanded project README added during scaffolding.
  - Resolution: Kept foundation/initial README (more complete, documents setup and CI). No content from Jules was required.

- .github/workflows/pr-ci-notify.yml
  - Conflict: Both branches added/edited this workflow in different commits.
  - Resolution: Kept foundation/initial version (validated and fixed to trigger on check_suite: completed). This version is functional and already validated.

Notes on other files:
- The Jules branch did not contain additional files beyond those now present in foundation/initial. The scaffold and CI workflow committed to foundation/initial include all required files from both branches.

Post-merge validation steps performed:
1. Validated GitHub Actions workflow YAML files (.github/workflows/*) for syntax and triggers.
2. Ensured package.json, tsconfig.json, next.config.ts, tailwind.config.ts, and app/ exist and are consistent.
3. Pushed commit to foundation/initial and triggered CI.

If you want a stricter 3-way merge record, I can re-run a file-by-file diff and attach the exact unified contents, but functionally foundation/initial now contains the merged content and CI has been triggered.
