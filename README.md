# Machine Learning for Computational Drug Discovery

[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter Notebooks](https://img.shields.io/badge/Jupyter-Notebooks-orange.svg)](https://jupyter.org/)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)
[![ChEMBL](https://img.shields.io/badge/Data-ChEMBL-green.svg)](https://www.ebi.ac.uk/chembl/)

## 📋 Overview

This project demonstrates a complete machine learning workflow for computational drug discovery using bioactivity data from the ChEMBL database. It provides a step-by-step approach to building predictive models that can accelerate the early stages of drug development by predicting how compounds will interact with specific biological targets.

By working through this project, you'll learn how to:
- Retrieve and process bioactivity data from public databases
- Analyze molecular properties and characteristics
- Calculate and interpret molecular descriptors
- Build and evaluate machine learning models for bioactivity prediction
- Compare different regression algorithms for QSAR modeling

## 🧪 Features

- **End-to-End Pipeline**: Comprehensive workflow from data acquisition to model evaluation
- **ChEMBL Integration**: Direct access to one of the largest public bioactivity databases
- **Molecular Analysis**: Calculation of Lipinski descriptors and advanced molecular fingerprints
- **Exploratory Data Analysis**: Visualization techniques for understanding chemical and biological patterns
- **Machine Learning Models**: Implementation of Random Forest and comparative analysis of multiple algorithms
- **Performance Metrics**: Thorough evaluation using R-squared, RMSE, and computational efficiency
- **Educational Focus**: Detailed explanations and comments to facilitate learning

## 📚 Project Structure

This project is organized as a series of Jupyter notebooks that guide you through the entire workflow:

| Notebook | Description |
|----------|-------------|
| **CDD_ML_Part_1_bioactivity_data.ipynb** | Retrieves and prepares bioactivity data from ChEMBL database using the `chembl_webresource_client` |
| **CDD_ML_Part_2_Exploratory_Data_Analysis.ipynb** | Performs exploratory data analysis including calculation of Lipinski's descriptors and visualization of property distributions |
| **CDD_ML_Part_3_Descriptor_Dataset_Preparation.ipynb** | Prepares the dataset by calculating molecular descriptors using PaDEL-Descriptor software |
| **CDD_ML_Part_4_Regression_Random_Forest.ipynb** | Builds and evaluates a Random Forest regression model for bioactivity prediction |
| **CDD_ML_Part_5_Compare_Regressors.ipynb** | Compares performance of multiple regression algorithms using the `lazypredict` library |

## 🚀 Getting Started

This project was developed in Google Colab, making it accessible without requiring local installation of dependencies or software.

### Running in Google Colab (Recommended)

The notebooks are designed to run in Google Colab and can be accessed directly:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

For each notebook:
1. Click the "Open in Colab" badge above or in each notebook
2. Make a copy to your own Google Drive (File → Save a copy in Drive)
3. Run the notebooks in sequence, as each builds upon the outputs of the previous one
4. Follow the installation instructions within each notebook for required libraries

The Google Colab environment provides all necessary computational resources and most required libraries are pre-installed or can be easily installed using `!pip install` commands included in the notebooks.

### Local Installation (Alternative)

If you prefer to run the notebooks locally:

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/ML-CDD.git
   cd Drug-Discovery
   ```

2. Create and activate a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Create a requirements file and install required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook
   # or
   jupyter lab
   ```

5. Open and run each notebook in sequence, starting with `CDD_ML_Part_1_bioactivity_data.ipynb`

## 📊 Data

This project uses data from ChEMBL, a manually curated database of bioactive molecules with drug-like properties. The specific focus is on:

- Bioactivity data for compounds tested against Acetylcholinesterase
- IC50 values converted to pIC50 (-log10(IC50)) for regression modeling
- Molecular descriptors calculated using PaDEL-Descriptor software

## 🧠 Machine Learning Models

The project implements and compares several regression models, including:

- Random Forest Regressor
- Multiple additional models via the `lazypredict` library
- Performance evaluation using R-squared, RMSE, and computation time

## 🔮 Future Directions

### Coming Soon: Web Application Deployment

The next phase of this project involves deploying the most effective predictive models as an interactive web application. This will allow researchers to:

- Input chemical structures or SMILES notations 
- Receive bioactivity predictions in real-time

**Repository:**  [bioactivity prediction app source code](https://github.com/zeineb-eya/bioactivity-predictions-app)

### Additional Future Developments

- Implementation of feature selection techniques to identify the most relevant molecular descriptors
- Extension to additional biological targets beyond Acetylcholinesterase
- Deep learning approaches for molecular representation and feature extraction
- Integration with molecular docking for validation of predictions
- Development of unsupervised learning methods for compound clustering


## 🙏 Acknowledgments

- ChEMBL database for providing open access to bioactivity data
- PaDEL-Descriptor software for molecular descriptor calculation
- Open source machine learning libraries including scikit-learn and lazypredict


