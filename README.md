# Xenium Breast Cancer Analysis

This repository contains notebooks for analyzing a Xenium In Situ dataset from a human breast cancer FFPE section.

## Dataset Source
The dataset used in this analysis is the Xenium In Situ dataset from a 0.4 cm² human breast cancer FFPE section, provided by 10x Genomics. It was downloaded from:

- [10x Genomics Xenium Preview Dataset](https://www.10xgenomics.com/products/xenium-in-situ/preview-dataset-human-breast)

The direct download link for the dataset is:
- [Xenium_FFPE_Human_Breast_Cancer_Rep1_outs.zip](https://cf.10xgenomics.com/samples/xenium/1.0.1/Xenium_FFPE_Human_Breast_Cancer_Rep1/Xenium_FFPE_Human_Breast_Cancer_Rep1_outs.zip)

To reproduce the analysis, download the dataset from the link above and extract it to the same location.

## Files in This Repository
- `Analyze_Xenium_data.ipynb`: Main analysis notebook for the Xenium dataset.

## Setup Instructions
To run the analysis, you need to set up a Python environment with the required dependencies. There are two options:

### Option 1: Use `environment.yml` (Recommended for Full Reproducibility)
This file contains the exact environment specification, including all dependencies.

1. Clone this repository:
   ```bash
   git clone https://github.com/BulutHamali/xenium-analysis-clean.git
   cd xenium-analysis-clean

2. Create a conda environment using environment.yml
   ```bash
   conda env create -f environment.yml
   conda activate xenium_env

3. Run the notebook in JupyterLab:
   ```bash
   jupyter lab

### Option 2: Use `requirements.txt` (Minimal Dependencies)
This file lists the key dependencies, which can be installed with pip.

1. Clone this repository (as above).

2. Create a conda environment and install dependencies:
   ```bash
   conda create -n xenium_env python=3.9
   conda activate xenium_env
   pip install -r requirements.txt

3. Run the notebook in JupyterLab (as above).
   


### Managing the `environment.yml` File

You can choose whether to include the `environment.yml` file in the repository for full reproducibility or ignore it if `requirements.txt` is sufficient.
### Option 1: Include `environment.yml` in the Repository (Recommended)

Add and commit the `environment.yml` file, then update the `README.md` with the instructions above.

   ```bash
   git add environment.yml README.md
   git commit -m "Add environment.yml and update README with instructions"
   git push
   ```

#### Option 2: Ignore `environment.yml`
If you don’t want to include `environment.yml` in the repository (e.g., because `requirements.txt` is sufficient), you can add it to `.gitignore` to prevent Git from tracking it.

1. Add `environment.yml` to `.gitignore`:

   ```bash
   echo "environment.yml" >> .gitignore
   ```

    Remove the file from your directory if you don’t need it:
    
     ```bash
     rm environment.yml
     ```
     
    
    Add and commit the updated `.gitignore`:
    
     ```bash
    git add .gitignore git commit -m "Update .gitignore to ignore environment.yml" 
    git push
    ```

### License

This project is licensed under the MIT License - see the  file for details.
