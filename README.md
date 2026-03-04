# Bioinformatics Portfolio

Focused showcase repository for three technical projects centered on sequence alignment, genomics data parsing, and computer-vision-based foreground extraction.

## Portfolio Goal

Present concrete, runnable work that demonstrates applied programming in adjacent technical domains without relying on unverifiable claims. Each project includes a working code path, example inputs, and documentation that explains the underlying method.

Dependability signals added across the portfolio:

- automated CI workflows per repository
- pinned runtime metadata through `pyproject.toml`
- explicit test suites and documented limitations
- verified output artifacts for parser and video runs

## Projects

### 1. PGx Sequence Aligner

Pairwise sequence alignment project with both CLI and API surfaces.

- Dynamic programming implementation for global and local alignment
- Adjustable match, mismatch, wildcard, and gap scoring
- Linear and affine gap models plus alignment statistics
- Focus areas: scoring matrices, traceback, and global versus local alignment

Repository:
https://github.com/Maxim-Firsov/pgx-sequence-aligner

### 2. Genomic Variant Parser

VCF processing utility that turns raw records into tabular summaries.

- Parses `GENE`, `IMPACT`, and `TRANSCRIPT` annotations
- Supports gzipped input and structured CSV/JSON exports
- Produces gene-level and variant-type summaries
- Focus areas: genomics file formats, normalization, and summary statistics

Repository:
https://github.com/Maxim-Firsov/genomic-variant-parser

### 3. Foreground Matting Video Mask

Classical computer-vision pipeline for generating subject masks from video.

- Auto profile for practical 4K processing plus background subtraction
- Mask cleanup, component filtering, and GrabCut refinement
- Emits run metadata describing the exact processing configuration
- Focus areas: frame differencing, segmentation heuristics, and temporal smoothing

Repository:
https://github.com/Maxim-Firsov/foreground-matting-video-mask

## Suggested Resume Framing

Use language tied to what these repositories actually demonstrate:

- Built a pairwise sequence alignment service supporting global and local alignment modes with configurable scoring.
- Developed a VCF parsing pipeline that converts variant records into gene-level and mutation-type summaries.
- Implemented a foreground-masking video pipeline using OpenCV stabilization, background subtraction, and matte refinement.
