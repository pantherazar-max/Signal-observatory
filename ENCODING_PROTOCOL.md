# Encoding Protocol v0.1

## Purpose

This document defines a reproducible, non-executable puzzle encoding. It is a teaching device, not cryptography.

## Layers

1. **Signal detection:** identify the three labeled data rows in the archive.
2. **Structural extraction:** preserve row labels and read each numeric triplet left to right.
3. **Symbol mapping:** use the published dictionary and grammar to interpret the recovered sequence.
4. **Integrity check:** compare the reconstructed phrase against the grammar validity checks.

## Numeric convention

Triplets are puzzle coordinates, not ASCII, Unicode, byte values, network ports, or instructions. Their mapping is defined only in the puzzle specification. Do not interpret them as commands or feed them to a shell, interpreter, or external service.

## Reproducibility

A solver should report:
- the rows selected,
- the order used,
- the mapping rule applied,
- the resulting NEXUS-Ω phrase,
- any ambiguity or alternative interpretation.

## Failure handling

If a value is missing or inconsistent, report the uncertainty. Do not silently substitute values or infer an undocumented rule.
