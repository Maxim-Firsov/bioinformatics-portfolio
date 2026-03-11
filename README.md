# Bioinformatics Projects

Collection of applied bioinformatics and adjacent engineering repositories spanning variant triage, sequence alignment, genomics data parsing, qPCR quality control, and lab-operations tooling.

Each project includes a working code path, example inputs, and documentation that explains the underlying method.

Common repository characteristics:

- automated CI workflows per repository
- pinned runtime metadata through `pyproject.toml`
- explicit test suites and documented limitations
- verified output artifacts for parser and video runs

## Projects

### 1. Variant Review Workbench (Pilot)

ClinVar-first small-variant triage and reporting tool for research-oriented review workflows.

- Parses VCF input and performs assembly-aware ClinVar matching
- Surfaces conflicting interpretations and submission evidence
- Applies transparent ranking and emits HTML/CSV/JSON outputs
- Optional PharmGKB enrichment for PGx context
- Focus areas: variant triage workflow design, reproducibility, and analyst-facing reporting

Repository:
https://github.com/Maxim-Firsov/variant-review-workbench

### 2. PGx Sequence Aligner

Pairwise sequence alignment project with both CLI and API surfaces.

- Dynamic programming implementation for global and local alignment
- Adjustable match, mismatch, wildcard, and gap scoring
- Linear and affine gap models plus alignment statistics
- Focus areas: scoring matrices, traceback, and global versus local alignment

Repository:
https://github.com/Maxim-Firsov/pgx-sequence-aligner

### 3. Genomic Variant Parser

VCF processing utility that turns raw records into tabular summaries.

- Parses `GENE`, `IMPACT`, and `TRANSCRIPT` annotations
- Supports gzipped input and structured CSV/JSON exports
- Produces gene-level and variant-type summaries
- Focus areas: genomics file formats, normalization, and summary statistics

Repository:
https://github.com/Maxim-Firsov/genomic-variant-parser

### 4. Foreground Matting Video Mask

Classical computer-vision pipeline for generating subject masks from video.

- Auto profile for practical 4K processing plus background subtraction
- Mask cleanup, component filtering, and GrabCut refinement
- Emits run metadata describing the exact processing configuration
- Focus areas: frame differencing, segmentation heuristics, and temporal smoothing

Repository:
https://github.com/Maxim-Firsov/foreground-matting-video-mask

### 5. qPCR HMM QC

Deterministic qPCR quality-control pipeline with HMM-style state calling and auditable outputs.

- Ingests RDML or canonical curve CSV
- Performs deterministic amplification-state inference
- Applies QC rules including NTC contamination and replicate discordance
- Emits CSV/JSON/HTML artifacts for review and audit

Repository:
https://github.com/Maxim-Firsov/qpcr-hmm-qc

### 6. Plate Transfer Audit

Plate transfer validation utility focused on operational quality checks in wet-lab workflows.

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
- `plate-transfer-audit`: MIT
- `qpcr-hmm-qc`: MIT
- `variant-review-workbench`: custom non-commercial, attribution-required license
