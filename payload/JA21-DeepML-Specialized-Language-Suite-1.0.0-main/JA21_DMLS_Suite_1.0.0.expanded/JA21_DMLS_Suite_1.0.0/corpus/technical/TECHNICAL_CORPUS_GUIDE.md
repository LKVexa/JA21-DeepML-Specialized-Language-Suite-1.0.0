
# DeepML Specialized Technical Corpus

## Purpose

This directory is the normalized technical heart of the standalone JA21 DeepML Specialized Language Suite. It reconstructs the uploaded 102-document wrapper into a searchable evidence system without discarding source, AST, semantic, compiler, runtime, validation, provenance, R12, MCRT, or Smithson 8S data.

## Contents

- `deepml_specialized_technical_corpus_10000.jsonl.gz` — all 10,000 normalized records.
- `specialized_01.jsonl.gz` through `specialized_20.jsonl.gz` — twenty 500-record shards.
- `technical_record.schema.json` — normalized record schema.
- `corpus_index.csv` — compact navigation and analysis index.

## Corpus profile

| Measure | Value |
|---|---:|
| Records | 10,000 |
| Topics | 42 |
| Tiers | 6 |
| Positive records | 7,875 |
| Ordinary diagnostic records | 1,125 |
| Certification holdouts | 1,000 |
| Expected stages | 5 |

## Record architecture

Each record separates identity, pedagogy, source, AST, semantics, compiler evidence, runtime evidence, optimization notes, validation, provenance, record-level coupling evidence, and the document-level 8S claim boundary. The `source_class` field preserves the original corpus classification; `publication_role` distinguishes ordinary diagnostics from certification holdouts.

## Specialized evidence discipline

A domain workflow is not valid merely because its output looks plausible. Units, shapes, schemas, provenance, adapter mappings, operator hashes, calibration state, constraints, causal order, network policy, actuation authority, domain inference, cross-domain conversions, and deterministic replay must remain explicit and testable.

## Native-evidence boundary

The corpus models expected compiler and runtime behavior. Native parsing, compilation, target lowering, domain execution, market or robotic actuation, graphics rendering, simulation, and replay require a conforming DeepML Specialized compiler and runtime, neither of which was supplied with the attachment.
