# OAE™ Engineering Standards

This repository is classified as test / integration infrastructure.

- Security first.
- Never commit credentials or production secrets.
- Keep external integrations explicit and isolated.
- Unit tests must not depend on hidden network state.
- Integration tests must declare their dependencies and failure modes.
- Make one coherent change at a time.
- Preserve existing behavior unless a contract change is intentional.
- Verify changes before acceptance.
- Do not describe test infrastructure as production-ready without evidence.

## OAE™ loop

```text
Observe → Understand → Plan → Implement → Test → Verify → Measure
```
