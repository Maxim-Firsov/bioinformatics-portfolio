# Bioinformatics Projects

Collection of applied bioinformatics and adjacent engineering repositories spanning variant triage, sequence alignment, genomics data parsing, qPCR quality control, and lab-operations tooling.

The active projects below include runnable code, example inputs, and documentation describing the underlying method.

## Projects

### 1. Variant Review Workbench (Pilot)

ClinVar-first small-variant triage and reporting tool for research-oriented review workflows.

- Parses VCF input and performs assembly-aware ClinVar matching
- Surfaces conflicting interpretations and submission evidence
- Applies transparent ranking and emits HTML/CSV/JSON outputs
- Optional PharmGKB enrichment for PGx context

Repository:
https://github.com/Maxim-Firsov/variant-review-workbench

### 2. PGx Sequence Aligner

Pairwise sequence alignment project with both CLI and API surfaces.

- Dynamic programming implementation for global and local alignment
- Adjustable match, mismatch, wildcard, and gap scoring
- Linear and affine gap models plus alignment statistics

Repository:
https://github.com/Maxim-Firsov/pgx-sequence-aligner

### 3. Genomic Variant Parser

VCF processing utility that turns raw records into tabular summaries.

- Parses `GENE`, `IMPACT`, and `TRANSCRIPT` annotations
- Supports gzipped input and structured CSV/JSON exports
- Produces gene-level and variant-type summaries

Repository:
https://github.com/Maxim-Firsov/genomic-variant-parser

### 4. Foreground Matting Video Mask

Classical computer-vision pipeline for generating subject masks from video.

- Auto profile for practical 4K processing plus background subtraction
- Mask cleanup, component filtering, and GrabCut refinement
- Emits run metadata describing the exact processing configuration

Repository:
https://github.com/Maxim-Firsov/foreground-matting-video-mask

### 5. qPCR Quality Control

Deterministic qPCR quality-control pipeline with HMM-style state calling and auditable outputs.

- Ingests RDML or canonical curve CSV
- Performs deterministic amplification-state inference
- Applies QC rules including NTC contamination and replicate discordance
- Emits CSV/JSON/HTML artifacts for review and audit

Repository:
https://github.com/Maxim-Firsov/qpcr-quality-control

### 6. Plate Transfer Audit (Inactive Draft)

Plate transfer validation utility focused on operational quality checks in wet-lab workflows.

This repository is not part of the current live portfolio rotation.

- Audits source-to-destination mapping consistency
- Detects transfer mismatches and rule violations
- Produces structured findings for downstream review

Repository:
https://github.com/Maxim-Firsov/plate-transfer-audit

## Licensing

Project licensing is explicit at the repository level:

- `bioinformatics-portfolio`: MIT
- `foreground-matting-video-mask`: MIT
- `genomic-variant-parser`: MIT
- `pgx-sequence-aligner`: MIT
- `plate-transfer-audit`: MIT, inactive draft
- `qpcr-quality-control`: MIT
- `variant-review-workbench`: Apache License 2.0
