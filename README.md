# Protein_Ligand_Interaction_Prediction_System
## Overview
This project presents a hybrid bioinformatics and deep learning framework for predicting drug–target interactions (DTIs) using molecular fingerprints and protein sequence-derived biochemical descriptors.The system integrates cheminformatics, bioinformatics, machine learning, and deep learning techniques to identify biologically significant inhibitor compounds against protein targets using real-world pharmacological datasets from BindingDB.The framework aims to accelerate early-stage computational drug discovery by predicting potential high-affinity interactions between chemical compounds and proteins.
----
## Objectives

- Predict drug–target interactions using computational methods
- Extract molecular fingerprints from chemical compounds
- Generate biochemical descriptors from protein sequences
- Compare traditional machine learning and deep learning approaches
- Identify biologically active compounds based on IC50 thresholds
- Visualize interaction patterns and active inhibitor compounds
----
## Dataset

The dataset was obtained from BindingDB, a public repository of experimentally validated drug–target interaction data.

### Dataset Includes:
- Ligand SMILES strings
- Protein amino acid sequences
- IC50 activity values
- Target protein information

### Preprocessing Performed:
- Removal of missing/invalid records
- Conversion of IC50 values into binary activity labels
- Dataset balancing to reduce target bias
----
## Methodology

### 1. Molecular Feature Extraction
Chemical compounds were converted into numerical representations using Morgan molecular fingerprints generated through RDKit.

### 2. Protein Feature Engineering
Protein sequences were analyzed using Biopython to extract biochemical descriptors such as:
- Molecular weight
- Aromaticity
- Instability index
- Hydrophobicity-related properties

### 3. Label Generation
Drug-target interactions were classified into:
- Active interactions
- Inactive interactions

based on IC50 activity thresholds.

### 4. Machine Learning Models
The project implemented:
- Random Forest Classifier
- Deep Neural Network

for comparative interaction prediction.

### 5. Evaluation Metrics
Model performance was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC score
----
## Technologies Used

### Programming Language
- Python

### Libraries & Frameworks
- TensorFlow / Keras
- Scikit-learn
- RDKit
- Biopython
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NetworkX
----
## Results

The framework successfully demonstrated the ability to:
- Predict biologically active drug-target interactions
- Differentiate strong and weak inhibitor compounds
- Identify potential high-affinity interactions
- Visualize interaction networks and molecular activity trends

The deep learning model showed improved predictive capability compared to baseline machine learning approaches under the selected feature engineering strategy.
----
## Workflow

BindingDB Dataset
        ↓
Data Cleaning & Preprocessing
        ↓
Molecular Fingerprint Generation
        ↓
Protein Feature Extraction
        ↓
Feature Integration
        ↓
ML & Deep Learning Training
        ↓
Drug-Target Interaction Prediction
        ↓
Biological Interpretation & Visualization
----
## Future Scope

Possible future improvements include:
- Transformer-based protein embeddings
- Graph neural networks for molecular representation
- Regression-based affinity prediction
- Molecular docking integration
- External benchmark validation
- Multi-class interaction prediction
----
## Applications

- Computational drug discovery
- Precision medicine research
- AI-assisted pharmacology
- Cancer therapeutics research
- Bioinformatics-based screening systems
----
## Working website: 
