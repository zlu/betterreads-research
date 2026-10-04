# AI-Assisted Literary Reading

**Author:** Zhao Lu  
**Date:** 2026-10-04  
**Canonical URL:** https://www.betterreads.dev/research/ai-assisted-literary-reading

## Abstract

BetterReads is an AI-assisted literary reading platform. Instead of summarizing books away, it attaches structured literary knowledge—characters, themes, glossary, timeline, and relationships—to the edition the reader is actually reading. This note states the problem, the design stance, and how the public research sample relates to the reading app.

## Problem

Difficult literature fails many readers not because the plot is unavailable in summary form, but because local reference breaks down: Who is speaking? What does this term mean here? Which theme is active in this chapter? Generic chatbots answer beside—or instead of—the book. BetterReads keeps help inside the reading session.

## Design stance

Stay inside the book. Annotation should increase the chance that a reader finishes a hard text, not substitute for reading it.

- Structured entities over free-form chat transcripts
- Chapter-aligned knowledge (timeline, theme intensity, glossary attestation)
- Public-domain corpora first, with clear provenance
- Scoped public samples for citation; larger editions available in the BetterReads reader

## System layers (conceptual)

At research granularity, BetterReads separates (1) edition text, (2) structured annotation graphs, (3) chapter companions / lenses as a reading UX, and (4) interactive Explain/Study tools. The v0.1 public sample focuses on (1) and a chapter-scoped slice of (2).

## Relation to the reading app

The BetterReads app applies this annotation model in a full reading environment—sync, PDF research reading, Study, and chapter companions. The research pages document the method and publish a small sample so the approach can be cited independently of the app.

## How to cite

Zhao Lu. *AI-Assisted Literary Reading*. BetterReads Research, 2026. https://www.betterreads.dev/research/ai-assisted-literary-reading
