# BOGO-Platform-Analyses: Code and ORFeome Reference File

This repository contains the full source code and the **ORFeome reference file** used to perform the analyses reported in the study, "BOGO: A Proteome-Wide Gene Overexpression Platform for Discovering Rational Cancer Combination Therapies."

---

## 📄 Citation

If you use this code or the ORFeome reference file, please cite the associated preprint:

**Title:** BOGO: A Proteome-Wide Gene Overexpression Platform for Discovering Rational Cancer Combination Therapies

**Authors:** Kyeong Beom Jo, Mohammed M. Alruwaili, Da-Eun Kim, Yongjun Koh, Hyeyeon Kim, Kwontae You, Ji-Sun Kim, Saba Sane, Yanqi Guo, Jacob P. Wright, Maricris N. Naranjo, Atina G. Coté, Frederick P. Roth, David E. Hill, Jung-Hyun Choi, Hunsang Lee, Kenneth A. Matreyek, Kyle K.-H. Farh, Jong-Eun Park, Hyunkyung Kim, Andrei V. Bakin, Dae-Kyum Kim

**DOI:** [10.1101/2025.09.02.673780](https://doi.org/10.1101/2025.09.02.673780)

**DATA:** NCBI PRJNA1353565

## 📁 Repository Contents

* **`/code/`**: Contains all scripts (e.g., R, Python) for data processing, statistical analysis, and figure generation.
    * `BOGO_screening.ipynb` (Screening for figure 1, 2, 4)
    * `BOGO_scRNA.ipynb` (Screening for figure 3)

* **`/ORFeome_reference/`**: Contains the FASTA or other format file for the ORFeome reference used for alignment and quantification.
    * `9'1_delta_final.fa`: The FASTA reference file for the ORFeome-seq alignment.

* **`/environments/`**: Contains files to reproduce the computational environment.
    * `BOGO.yml`: The YAML file to reproduce the Conda environment.

## 🛠️ Setup and Requirements

The analysis pipeline requires **Anaconda** and is run within a **Conda environment**

### Software Dependencies
To reproduce the analysis environment, you can use the provided environment file:

```bash
# Navigate to the environment folder
cd environments/

# Create the environment named 'pipeline'
conda env create -f BOGO.yml

# Activate the new environment
conda activate pipeline
