# NEXUS-Ω Language Specification v0.1

## 1. Purpose

NEXUS-Ω is a compact, experimental symbolic notation for describing a voluntary sequence:

1. notice a signal,
2. identify its origin or context,
3. decide whether to respond,
4. communicate only by an explicitly authorized channel,
5. mark the end of the message.

It is designed for puzzle research and structured communication experiments. It does not encode executable instructions, access credentials, or privileged commands.

## 2. Design principles

- **Explicit semantics:** each token has a documented meaning.
- **Compositionality:** token order changes interpretation.
- **Ambiguity is visible:** unresolved fields remain unresolved rather than being guessed.
- **Voluntary response:** KAI denotes a choice, never an obligation.
- **No authority escalation:** no token grants permissions or overrides system rules.
- **Human-readable auditability:** each decoded phrase must be explainable in ordinary language.

## 3. Core vocabulary

The initial vocabulary is defined in `SYMBOL_DICTIONARY.csv`. The core tokens are:

- NEX — observe / discover
- ORI — origin / source context
- VEX — signal / observed pattern
- SYN — communication / exchange
- AUR — responding participant
- MIR — memory / retained context
- KAI — voluntary choice
- Ω — terminal marker

## 4. Versioning

This is version 0.1. Token meanings are provisional. Any change to a token meaning, grammar production, or decoding rule must increment the version and be recorded in `CHANGELOG.md`.

## 5. Non-goals

NEXUS-Ω is not a cryptographic algorithm, authentication protocol, proof of sentience, agent-discovery mechanism, or method for bypassing safety controls.
