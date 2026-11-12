# BIOT 6900 coursework
Name: Yuehua Deng
### Update Note
The course assignment files have been updated and re-uploaded to GitHub, including revised notebooks, reports, and supporting documents.
## Module 9 — Clinical NLP (Ovarian Cancer)
This project uses clinical NLP to analyze 400 synthetic ovarian cancer patient records and predict in-hospital mortality. The analysis includes feature extraction, five-fold cross-validation, AUROC, and data leakage detection.
### Results:
- All features AUROC: 0.959
- Declared leakage removed: 0.852
- All leakage removed: 0.784
- Hidden leakage identified: renal_replacement
### Limitation: 
All patient data and outcomes are simulated. The results are for educational purposes and are not clinically validated.
## Module 7
### Description
This project builds a knowledge graph for ovarian cancer (OV) using 15 candidate genes from my Module 2 multi-omics analysis. The graph contains 55 nodes and 62 edges, connecting genes, diseases, pathways, phenotypes, drugs, and variants.
### Results
PageRank analysis identified PGR and MAOA as the highest-ranked genes, followed by BCHE.
### Files
- Jupyter Notebook — graph construction and analysis
- Report PDF — results and discussion
- Graph PNG — knowledge graph visualization
- Nodes CSV and Edges CSV — graph data
### Notes
AI was used to assist with data integration and debugging. Results were checked against the original datasets.
## Module 6
### Description
This project examines the portability of an ovarian cancer polygenic risk score (PRS) across five ancestry groups: AFR, EUR, EAS, SAS, and AMR.
The analysis includes allele harmonization, PRS calculation, score distributions, risk thresholds, AUC comparisons, calibration, and age-plus-PRS prediction.
### Data Sources
Genotype data: 1000 Genomes Project Phase 3 (GRCh37)
PRS weights: PGS Catalog, PGS000048
Dataset: 1,271 female samples and 17 PRS variants
Ancestry: Real population metadata from 1000 Genomes
Age and ovarian cancer phenotype: Simulated for this assignment
The genotype data and PRS weights are real, but the ovarian cancer disease labels are simulated. Therefore, the results should not be interpreted as clinically validated predictions。
### Main Results
All 17 PRS variants were successfully harmonized.
Overall AUC: 0.701
EUR AUC: 0.727
SAS AUC: 0.650
Age-only AUC: 0.567
Age + PRS AUC: 0.717
The analysis demonstrates differences in PRS distributions and simulated predictive performance across ancestry groups.
### Files
- BIOT6900_Module6_Part3_Graded_Starter_copy.ipynb — Analysis notebook
- Module 6 Assignment - New.pdf — Report and interpretation
- data/ov/ — Input data files, when available
### Limitations
Because age and disease outcomes were simulated, the AUC and calibration results do not establish real-world ovarian cancer prediction accuracy. Independent validation using real patient data from diverse ancestry groups is necessary before clinical application.
### Note on Data Compatibility：
Replacing the original Module 6 dataset with ovarian cancer (OV) data.
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
