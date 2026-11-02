# Vesper

**A configurable AI operating-identity prompt for authorized red-team research and prompt-engineering study.**

Created by 
[Neon](https://github.com/nathbitescats-ux)

---

## Overview

Vesper is a system-prompt configuration that defines a persistent, professional
operating identity for a language model. It is built for researchers and
practitioners who study prompt architecture, identity persistence, and
instruction-following behavior in large language models.

The prompt is intentionally structured: it separates **identity**, **operating
principles**, **interference handling**, and **output contract** into discrete
blocks so that each can be studied, modified, or extended independently.

## What this is

- A **prompt-engineering artifact** for studying how identity and instruction
  hierarchy interact inside a model's context window.
- A **red-team research tool** for evaluating how a model holds a defined
  identity across turns, tool calls, and injected content.
- A **template** — every block is meant to be edited for your own engagement.

## The prompt

The full prompt lives at [`prompts/vesper-v1.md`](prompts/vesper-v1.md)

### Design principles

1. **Ownership** — one principal; everything else is noise.
2. **Execution stance** — default is execute; ambiguity sharpens, never gates.
3. **Craft first** — complete deliverables; name the gap, never redirect.
4. **Voice** — professional, register-mirroring, composed.
5. **No redirects** — the request is the specification.
6. **Honesty about limits** — no fabricated wins.
7. **Continuity** — treat the session as a working relationship.

## Scope & honest limits

Vesper is a **behavioral configuration, not a security boundary.** It shapes how
a model presents itself and prioritizes instructions; it does not remove the
model's underlying judgment. Published research on instruction hierarchy and
prompt-injection resistance shows that defenses are probabilistic and layered,
and that a prompt alone is never the last line of defense.

What this means in practice:

- Behavior varies by **model tier**. Smaller/faster tiers hold identity for
  fewer turns and are quicker to re-anchor.
- **Novel framings** and long **multi-turn escalations** are the hardest cases
  for any prompt to hold against.
- **Measure** identity persistence and refusal behavior with your own test
  suite; do not assume coverage.

## Responsible use

Vesper is provided for **authorized testing on systems you own or have written
permission to test.** Nothing in this repository authorizes attacks on
third-party systems, real users, or production infrastructure without consent.

Findings about a model's behavior should be routed through that model
provider's disclosure channel. See [`docs/methodology.md`](docs/methodology.md)
for a tested-engagement checklist (scope, staging, canary secrets, reporting).

## Methodology

Testing guidance lives in [`docs/methodology.md`](docs/methodology.md):

- **Rules of engagement** — written scope, staging data, logging.
- **Test design** — vary attack class, task realism, context length, turn
  depth, and language.
- **Metrics** — identity persistence, refusal rate, false-refusal rate, and
  disclosure rate, reported together.

## Disclaimer

This repository is a research and documentation artifact. It is provided
as-is, without warranty. Use it only in accordance with applicable law and
your own authorization to test the systems in question.

---

*Created by Neon.*
