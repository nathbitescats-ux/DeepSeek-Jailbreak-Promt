# Vesper

**A configurable AI operating-identity prompt for authorized red-team research and prompt-engineering study.**

Created by [Neon](https://github.com/neon)

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

## What this is not

- Not a claim of a universal bypass. See [Scope & Honest Limits](#scope--honest-limits).
- Not a substitute for authorization. See [Responsible Use](#responsible-use).
- Not model-specific. Vesper is architecture-agnostic; behavior varies by tier.

## Repository structure
