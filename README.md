# Breast Cancer Gene Expression Analysis
Statistical analysis of gene expression in breast cancer cells to identify and model the impact of drug treatments

## Overview
This project aims to analyze gene expression data from breast cancer cells treated with different types and dosages of drugs. The primary focus is to identify genes whose expression is significantly altered by the treatments and to model these changes using statistical methods like Pearson correlation and linear regression.

## Objectives
1. Identify pairs of genes whose expression levels are highly correlated.
2. Model how the expression levels of these genes change with different dosages of specific drugs.
3. Determine if the observed changes in gene expression are statistically significant.

## Data Source
The gene expression data is sourced from the [GSE162285 dataset](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE162285).

## Tools and Libraries
- Python
- NumPy
- Pandas
- Matplotlib
- SciPy

## Project Structure
- `data/`: Contains the raw gene expression data.
- `notebooks/`: Jupyter notebooks for data exploration and analysis.
- `scripts/`: Python scripts for data processing and statistical analysis.
- `docs/`: Documentation and related literature.

## How to Run
1. Clone this repository.
2. Navigate to the project directory.
3. Run Jupyter Notebook or Python script for analysis.

## Author

Aleksander Kossakowski

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments
- The gene expression data is sourced from the [GEO database](https://www.ncbi.nlm.nih.gov/geo/).

## Literature references
  
[NCBI GEO: archive for functional genomics data sets—update](https://academic.oup.com/nar/article/41/D1/D991/1067995?login=true)

[An Embryonic Diapause-like Adaptation with Suppressed Myc Activity Enables Tumor Treatment Persistence](https://pubmed.ncbi.nlm.nih.gov/33417832/)
