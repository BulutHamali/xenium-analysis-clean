# Xenium Breast Cancer Analysis
This repository contains notebooks for analyzing a Xenium In Situ dataset from a human breast cancer FFPE section.
Dataset Source

The dataset used in this analysis is the Xenium In Situ dataset from a 0.4 cm² human breast cancer FFPE section, provided by 10x Genomics. It was downloaded from:

    10x Genomics Xenium Preview Dataset

The direct download link for the dataset is:

    Xenium_FFPE_Human_Breast_Cancer_Rep1_outs.zip
Files in This Repository

    Analyze_Xenium_data.ipynb: Main analysis notebook for the Xenium dataset.

Setup Instructions

To run the analysis, you need to set up a Python environment with the required dependencies. See the requirements.txt file for a list of dependencies.

Clone this repository:

git clone https://github.com/BulutHamali/xenium-analysis-clean.git
cd xenium-analysis-clean


Create a conda environment and install dependencies:


conda create -n xenium_env python=3.9
conda activate xenium_env
pip install -r requirements.txt

jupyter lab


License

This project is licensed under the MIT License - see the  file for details.

