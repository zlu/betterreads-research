# Structured Literary Annotation

**Author:** Zhao Lu  
**Date:** 2026-10-04  
**Canonical URL:** https://www.betterreads.dev/research/structured-literary-annotation

## Abstract

This note defines the BetterReads structured literary annotation model: canonical chapter identifiers, entity types, and how chapter-scoped samples are exported for research. It is the formal counterpart to the v0.1 public dataset.

## Canonical chapter identity

All annotations reference `chapter_id` values of the form `NNNN-slug` (zero-padded spine order plus title slug). Timeline events, character first appearances, and theme×chapter scores share this key so researchers can align layers without fuzzy title matching.

## Entity types

The research schema exposes a stable subset of annotation fields, flattened to plain English strings for portability.

- **characters** — id, name, aliases, importance, first_appearance, short_bio, snapshot
- **themes** — id, name, description; plus theme×chapter scores
- **timeline** — narrative events with chapter_id and characters_involved
- **glossary** — term + explanation for items attested in the selected chapter
- **relationships** — node/edge subgraph among included characters

## Export method (v0.1)

For each selected chapter we include public-domain plain text from the ingested edition; characters linked by first appearance, timeline involvement, or major-name attestation; glossary terms from chapter key-term hints and in-text matches; and relationship edges among the retained character set. Companion prose is documented separately and is not part of this sample.

## Machine-readable schema

JSON Schema: [`../literary-annotation-v0.1/schema/literary-annotation.schema.json`](../literary-annotation-v0.1/schema/literary-annotation.schema.json)

## How to cite

Zhao Lu. *Structured Literary Annotation*. BetterReads Research, 2026. https://www.betterreads.dev/research/structured-literary-annotation
