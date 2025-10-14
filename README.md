# AI-driven prediction of lung cancer patient responses to immunotherapy

## Abstract
Lung cancer remains one of the leading causes of cancer-related mortality worldwide, and
the advent of immunotherapy has significantly improved survival outcomes for a subset
of patients. However, accurately predicting treatment response remains a major clinical
challenge due to the complexity and heterogeneity of patient profiles.
In this thesis, we explore an AI-driven predictive framework for modeling and interpreting patient responses to immunotherapy, based on a retrospective cohort including
demographic, clinical, and molecular features. Multiple clinically relevant endpoints are
investigated, encompassing both survival and response indicators: **Overall Survival
(OS)** status and duration, **Progression-Free Survival (PFS)**, **Time to Progression
(TTP)**, **Best Overall Response (BOR)** and its modified variants, as well as **Responder Quality Groups** derived from both raw and log-transformed TTP.
Three main modeling paradigms, *classical machine learning*, *conventional neural
networks*, and *advanced neural architectures*, are systematically compared. Through
targeted hyperparameter tuning and regularization, we mitigate overfitting and show that
model complexity should be adapted to each endpoint rather than uniformly increased.
Model interpretability is ensured through *SHAP-based feature* attributions, which
identify biologically plausible predictors of treatment outcome. Finally, ethical and sustainability aspects are discussed, highlighting the social and economic value of AI-assisted
decision support in clinical oncology, despite the environmental costs of model training.
Overall, this work demonstrates that interpretable and endpoint-specific AI models can
effectively complement clinical expertise, improving patient stratification and promoting
a more personalized and sustainable approach to lung cancer immunotherapy

## Thesis Context
This repository contains the code and experiments developed for my Master's thesis in Data Science, focused on applying machine learning and deep learning techniques to predict lung cancer patients' responses to immunotherapy.  
The work was conducted in collaboration with *Hospital Clínic de Barcelona* within a multidisciplinary research environment combining clinical data analysis and artificial intelligence.

## Datasets
The code in this repository reflects the original analysis pipeline used during the thesis, including preprocessing, feature engineering, and model training steps.  
For confidentiality reasons, the clinical datasets themselves **are not included**, as they belong to *Hospital Clínic de Barcelona* and contain sensitive patient information.  
Nonetheless, all variable names, preprocessing routines, and modeling workflows are left exactly as implemented in the original project, so that readers can fully understand and reproduce the structure of the analysis using their own data.  
Researchers with legitimate scientific interest and institutional authorization may request access to the original datasets.  

## Repository Description
This repository contains the implementation notebooks developed for my Master’s Thesis.  
The project investigates multiple clinically relevant endpoints, **Overall Survival (OS)**, **Progression-Free Survival (PFS)**, **Time to Progression (TTP)**, **Best Overall Response (BOR)** and **Responder Quality Groups**, using a combination of classical machine learning algorithms, conventional neural networks, and advanced deep learning architectures (including attention mechanisms).  
Each folder under `notebooks/` corresponds to a target endpoint and contains four implementation notebooks:  
1. `classic_ml/` — traditional machine learning models (e.g., SVM, Random Forest, XGBoost)
2. `conventional_nn/` — fully-connected neural networks  
3. `advanced_nn/` — DL architectures   
4. `attention_nn/` — attention-based neural networks  
Preprocessing (mainly scaling) is applied when required by the model type (for example tree-based methods use raw feature inputs).\\
For each model, SHAP value visualizations are provided to support interpretability.

### Repository Structure
├── notebooks/  
│ ├── OS_status/  
│ │ │ ├── classic_ml/  
│ │ │ ├── conventional_nn/  
│ │ │ ├── advanced_nn/  
│ │ │ ├── attention_nn/  
│ │   
│ ├── OS_duration/   
│ │ │ ├── ...  
│ │    
│ ├── PFS/  
│ │ │ ├── ...  
│ │  
│ ├── TTP/  
│ │ │ ├── ...  
│ │  
│ ├── BOR_original/  
│ │ │ ├── ...  
│ │   
│ │ ├── BOR_no_CR/  
│ │ │ ├── ...  
│ │   
│ │ ├── BOR_CR_into_PR/  
│ │ │ ├── ...  
│ │  
│ ├── RespGroup_from_TTP/  
│ │ │ ├── ...  
│ │   
│ │ ├── RespGroup_from_logTTP/  
│ │ │ ├── ...  
│ │   
├── Noemi_Cicala_thesis.pdf  
└── README.md  

## Requirements
```
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install tensorflow
pip install shap
pip install imbalanced-learn
pip install scikit-learn
pip install xgboost
pip install lightgbm
```
These dependencies have been tested with **Python 3.11**.  
Compatibility with later versions (e.g., 3.12+) may vary depending on library updates.
