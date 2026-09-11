# iCAMP community assembly analysis

This directory contains the input data, R workflow, and principal outputs used to evaluate bacterial community assembly processes with iCAMP.

## Directory structure

### `input`

Input files used for the iCAMP analysis:

- `asv_table.txt`  
  ASV count table generated from MicrobiomeAnalyst export.

- `asv_taxonomy.txt`  
  Taxonomic classification associated with each ASV.

- `tree.nwk`  
  Phylogenetic tree used to calculate pairwise phylogenetic distances.

- `sample-metadata.txt`  
  Physicochemical variables associated with each composite sample.

- `treat2col.txt`  
  Treatment assignment used by iCAMP (`C` = *Cyperus articulatus*, `T` = *Thalia geniculata*, and `U` = unplanted treatment).

### `script`

- `iCAMP.Rmd`  
  R workflow used to prepare the iCAMP input files, evaluate within-bin phylogenetic signal, perform phylogenetic binning, and estimate ecological assembly processes.

### `output`

Principal iCAMP outputs used in the manuscript:

- `wetlands.ProcessImportance_EachGroup.csv`  
  Relative contributions of ecological processes within each planted treatment and between treatments.

- `wetlands.ProcessImportance_EachTurnover.csv`  
  Process contributions for each pairwise community turnover.

- `wetlands.ProcessImportance_EachBin_EachGroup.csv`  
  Process contributions resolved by phylogenetic bin.

- `wetlands.BinContributeToProcess_EachGroup.csv`  
  Contribution of individual bins to each ecological process.

- `wetlands.Taxon_Bin.csv`  
  Assignment of ASVs to phylogenetic bins.

- `wetlands.Bin_TopTaxon.csv`  
  Taxonomic summary of each phylogenetic bin.

- `wetlands.PhyloSignalSummary.csv` and `wetlands.PhyloSignalDetail.csv`  
  Outputs from the within-bin phylogenetic-signal assessment.

## Sample inclusion

The original ASV table contained five composite samples: two associated with *C. articulatus*, two with *T. geniculata*, and one unplanted sample.

Because within-treatment community turnover requires at least two independent samples, the unplanted treatment was excluded from the iCAMP analysis. ASVs with zero abundance across the four remaining planted samples were subsequently removed. Process proportions are therefore interpreted descriptively rather than as inferential treatment-level estimates.
