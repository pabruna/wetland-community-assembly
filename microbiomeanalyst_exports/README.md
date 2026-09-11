# MicrobiomeAnalyst exports

This directory contains the ASV-level tables exported from MicrobiomeAnalyst and used as the starting point for downstream analyses.

The files correspond to the dataset obtained after sequence processing and ASV inference with DADA2, but prior to filtering performed within MicrobiomeAnalyst for selected downstream analyses.
Raw sequencing reads are available through the NCBI Sequence Read Archive (BioProject PRJNA1285480).

## Files

- `microbiomeAnalyst_asv_seq.txt`  
  ASV nucleotide sequences and sample-level read counts. The table contains 3,732 ASVs across five composite samples.

- `microbiomeAnalyst_taxonomy_annotation.txt`  
  Taxonomic assignments corresponding to the same 3,732 ASV sequences.

- `microbiomeAnalyst_16s_abund.txt`  
  Taxonomy-labelled ASV abundance table corresponding to the same dataset.
