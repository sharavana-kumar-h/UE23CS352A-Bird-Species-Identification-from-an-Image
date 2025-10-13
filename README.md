# Bird Species Identification from an Image

**UE23CS352A – Machine Learning Mini Project**  
**Team Members:** Sharavana Kumar H, Nishita Singh  
**Date:** 13th October 2025  

---

## Project Overview

This project applies Machine Learning techniques to identify bird species from images using the **Caltech-UCSD Birds-200-2011 (CUB-200)** dataset.  
The model distinguishes between visual features such as color, shape, and texture of bird parts, classifying each input image into one of multiple bird species.

**Objectives:**

- Data preprocessing and feature extraction from images  
- Applying and comparing ML algorithms (SVM, Logistic Regression, Random Forest, etc.)  
- Model evaluation and visualization using confusion matrices and accuracy plots  

---

## Repository Structure
UE23CS352A-Bird-Species-Identification-from-an-Image/   
├── Classifier-Code.ipynb # Additional experiments with classifiers                                                                                                                                                                                                                                                                                                                                         
├── ML_MiniProject.ipynb # Main notebook: preprocessing, training, evaluation                                                                                                                                     
├── Project_Summary.pdf                                                                                                                                                                                           
└── README.md 

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/sharavana-kumar-h/UE23CS352A-Bird-Species-Identification-from-an-Image.git
cd UE23CS352A-Bird-Species-Identification-from-an-Image
```
### 2. Create a Virtual Environment (Recommended)
```bash
python -m venv ml_env
# Activate the environment
source ml_env/bin/activate      # Linux/Mac
ml_env\Scripts\activate         # Windows
```
### 3. Install Dependencies
```bash
pip install -r requirements.txt
```
If requirements.txt is missing, install manually:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn opencv-python
```
### 4. Dataset Setup

- Download the CUB-200-2011 dataset
- Extract and place the dataset inside the project root:

```bash
data/CUB_200_2011/
```

### Running the Project
**Using Jupyter Notebook**
```bash
jupyter notebook
```
- Open ML_MiniProject.ipynb
- Run all cells sequentially to:
  - Preprocess the data
  - Train models (KNN, SVM, LDA, Logistic Regression, etc.)
  - Evaluate performance and visualize results

---

### Key Learnings

- Feature extraction and dimensionality reduction (PCA, feature selection) significantly improved accuracy.

- Logistic Regression performed best for this high-dimensional, multi-class classification problem.

- Implementing multiple algorithms deepened understanding of model trade-offs.

---

### References:
  - Title: "The Caltech-UCSD Birds-200-2011 Dataset"                                                                                                                                                             
    Authors: "C. Wah et al."                                                                                                                                                                                     
    Source: "Caltech Technical Report CNS-TR-2011-001"                                                                                                                                                           
    Link: "https://gwern.net/doc/ai/dataset/2011-wah.pdf"                                                                                                                                                        

  - Title: "Scikit-learn: Machine Learning in Python"                                                                                                                                                            
    Authors: "F. Pedregosa et al."                                                                                                                                                                               
    Source: "Journal of Machine Learning Research, 2011"                                                                                                                                                         
    Link: "https://www.jmlr.org/papers/volume12/pedregosa11a/pedregosa11a.pdf"                                                                                                                                                                                                                                                                                            

  - Title: "Bird Species Categorization Using Pose Normalized Deep Convolutional Nets"                                                                                                                           
    Authors: "S. Branson et al."                                                                                                                                                                                 
    Source: "2014"                                                                                                                                                                                               
    Link: "https://arxiv.org/pdf/1406.2952"                                                                                                                                                                      

