# BIOT 6900 coursework

Name: Yuehua Deng

## Multi-Omics Target Discovery in Ovarian Cancer

### Disease
Ovarian cancer

## Data Sources

### 1. Transcriptomics
- Dataset: E-GEOD-40595
- Data type: Differential gene expression
- Comparison used: ovarian cancer vs normal in epithelial cells
- Platform: Expression Atlas
- Columns used:
  - gene
  - log2 fold change
  - p-value
- Access: Open
- Source:
  https://www.ebi.ac.uk/gxa/experiments/E-GEOD-40595

### 2. Proteomics
- Dataset: CPTAC pan-cancer ovarian cancer cohort
- Data type: Gene-level proteomics
- Groups used:
  - Proteomics (Tumor)
  - Proteomics (Normal)
- Effect calculation:
  mean tumor protein abundance - mean normal protein abundance
- Statistical test:
  Welch's t-test
- Access: Open
- Source:
  https://www.linkedomics.org/data_download/CPTAC-pancan-OV/

### 3. Genomics
- Dataset: CPTAC pan-cancer ovarian cancer cohort
- Data type: Gene-level somatic mutation
- Genomic evidence:
  mutation frequency across tumor samples
- Access: Open
- Source:
  https://www.linkedomics.org/data_download/CPTAC-pancan-OV/

## Analysis Overview

The three omics layers were reduced to one row per gene.

- Transcriptomics: gene, RNA log2 fold change, RNA p-value
- Proteomics: gene, protein effect, protein p-value
- Genomics: gene, mutation frequency

Gene identifiers were harmonized to gene symbols, and the three layers were joined by gene.

RNA-protein concordance was defined by direction agreement between RNA log2 fold change and protein effect.

A multi-evidence score was calculated using equal weights across transcriptomic, proteomic, and genomic evidence.

The top-ranked genes were exported to:

`targets_ov.csv`

## Output Files

- `BIOT6900_Module2_Starter_OV.ipynb`
- `targets_ov.csv`

## Notes

The transcriptomic and proteomic datasets come from different cohorts and are therefore integrated at the gene level rather than at the matched-sample level.

The CPTAC ovarian RNA tumor-only expression matrix was explored during data selection but was not used in the final transcriptomic scoring because it did not provide a tumor-vs-normal effect and p-value.
- `BIOT6900_Module2_Assignment2_OV.ipynb`
- `report.pdf`
