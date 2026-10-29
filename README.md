# BIOT 6900 coursework
Name: Yuehua Deng
## Module 6
### Description
This assignment examines the portability of polygenic risk scores (PRS) across ancestry groups using real 1000 Genomes genotype data and a published Alzheimer's disease PRS (PGS000334).
The analysis includes allele harmonization, PRS calculation, ancestry-specific score distributions, high-risk classification thresholds, AUC comparisons, and calibration.
### Data Sources
- genotypes.csv – Genotype data
- variants.csv – Variant information
- meta.csv – Sample metadata and ancestry information
- score.csv – PRS scoring information (PGS000334, Alzheimer's disease)
### Note on Data Compatibility：
My selected disease for the course is ovarian cancer (OV). I downloaded an ovarian cancer PRS from the PGS Catalog (PGS000048) and compared its variants with the provided genotype panel.
The comparison showed 0 overlapping variants, so the ovarian cancer PRS could not be calculated using the supplied files.
Therefore, I completed the notebook and report using the Alzheimer's disease score (PGS000334) included in the provided dataset, as specified in the graded starter notebook. The results illustrate PRS portability across ancestry groups and should not be interpreted as ovarian cancer risk predictions.
## Module 5
### Research gene:CYP2C19
This repository contains my completed Module 5 variant interpretation assignment.
### Description:
In this module, I analyzed CYP2C19 variants using CADD, REVEL, AlphaMissense, and AlphaGenome Atlas. I evaluated prediction-tool coverage, applied an allele-frequency filter, attempted CADD calibration, and examined discordant prediction results.
### Data Sources:
MyVariant.info and ClinVar.
gnomAD.
CADD, REVEL, and AlphaMissense.
AlphaGenome Atlas
The submitted files include the completed Jupyter Notebook, the classified variant CSV file, and the report PDF.
## Module 4 
Targets: PGR and BCHE
This repository contains my Module 4 assignment for structure prediction and structure-based druggability analysis.
### Description:
In this module, I analyzed the predicted protein structures of PGR and BCHE. I evaluated structural confidence using pLDDT and PAE, compared predicted structures with experimental structures, and assessed potential binding pockets using fpocket.
### Data Sources:
AlphaFold Protein Structure Database: PGR and BCHE predicted structures.
Protein Data Bank (PDB): experimental structures 1A28 and 6QAA.
Previously prioritized targets from Modules 2 and 3.
### Files:
BIOT6900_Module4_Assignment.ipynb
structure_assessment_ov.csv — summary of the structural assessment
Module 4 Assignment.pdf
## Module 3 
Disease: OV
### Description:
In this module, I evaluated the tractability of ovarian cancer candidate targets using protein sequence-based predictions. I combined disease relevance and tractability priors using a 60% and 40% weighting, and compared small-molecule and antibody tractability scores.
### Data Sources:
Candidate targets and multi-omics scores from my Module 2 analysis.
Protein sequence information and tractability prediction results from the Module 3 workflow.
### Files included:
- BIOT6900_Module3_Assignment.ipynb
- targets_ov_w3.csv
- Module 3 Assignment — Computational Lab 3.pdf
Notes:
All top 15 targets were successfully mapped to the reviewed human proteome. The notebook ran successfully and the Module 3 analysis was completed.
## Module 2 
### Disease
Ovarian cancer
### Data Sources
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

The CPTAC ovarian RNA tumor-only expression matrix was explored during data selection but was not used in the final transcriptomic scoring because it did not provide a tumor-vs-normal effect and p-value.
## Module 1 
Parts A–C completed.
Part D will be covered in the next class.
