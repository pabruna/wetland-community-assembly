# Constructed wetland bacterial community assembly

This repository contains the processed input data, analysis scripts, and reference outputs used to evaluate bacterial community assembly with iCAMP in pilot-scale constructed wetlands planted with *Cyperus articulatus* (Ca) and *Thalia geniculata* (Tg).

## Repository structure

```text
.
├── data/
│   └── microbiomeanalyst_exports/
│       ├── README.md
│       ├── microbiomeAnalyst_asv_seq.txt
│       ├── microbiomeAnalyst_taxonomy_annotation.txt
│       └── microbiomeAnalyst_16s_abund.txt
│
└── iCAMP/
    ├── README.md
    │
    ├── input/
    │   ├── asv_table.txt
    │   ├── asv_taxonomy.txt
    │   ├── sample-metadata.txt
    │   ├── treat2col.txt
    │   └── tree.nwk
    │
    ├── script/
    │   └── iCAMP.Rmd
    │
    └── output/
        ├── wetlands.ProcessImportance_EachGroup.csv
        ├── wetlands.ProcessImportance_EachTurnover.csv
        ├── wetlands.ProcessImportance_EachBin_EachGroup.csv
        ├── wetlands.BinContributeToProcess_EachGroup.csv
        ├── wetlands.Taxon_Bin.csv
        ├── wetlands.Bin_TopTaxon.csv
        ├── wetlands.PhyloSignalSummary.csv
        └── wetlands.PhyloSignalDetail.csv

```
### Samples

NCBI SRA BioProject **PRJNA1285480**

Five composite microbiome samples are present in the processed ASV table:

- `CaS3_S35_L001` — *Cyperus articulatus*
- `CaS4_S47_L001` — *Cyperus articulatus*
- `TgS1_S11_L001` — *Thalia geniculata*
- `TgS2_S23_L001` — *Thalia geniculata*
- `UpS5_S59_L001` — unplanted control

The original treatment file encodes these groups as `C`, `T`, and `U`, respectively.
