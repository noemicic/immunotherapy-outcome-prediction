# AI-driven prediction of lung cancer patient responses to immunotherapy

## Abstract
Lung cancer remains one of the leading causes of cancer-related mortality worldwide, and
the advent of immunotherapy has significantly improved survival outcomes for a subset
of patients. However, accurately predicting treatment response remains a major clinical
challenge due to the complexity and heterogeneity of patient profiles.
In this thesis, we explore an AI-driven predictive framework for modeling and interpreting patient responses to immunotherapy, based on a retrospective cohort including
demographic, clinical, and molecular features. Multiple clinically relevant endpoints are
investigated, encompassing both survival and response indicators: Overall Survival
(OS) status and duration, Progression-Free Survival (PFS), Time to Progression
(TTP), Best Overall Response (BOR) and its modified variants, as well as Responder Quality Groups derived from both raw and log-transformed TTP.
Three main modeling paradigms, classical machine learning, conventional neural
networks, and advanced neural architectures, are systematically compared. Through
targeted hyperparameter tuning and regularization, we mitigate overfitting and show that
model complexity should be adapted to each endpoint rather than uniformly increased.
Model interpretability is ensured through SHAP-based feature attributions, which
identify biologically plausible predictors of treatment outcome. Finally, ethical and sustainability aspects are discussed, highlighting the social and economic value of AI-assisted
decision support in clinical oncology, despite the environmental costs of model training.
Overall, this work demonstrates that interpretable and endpoint-specific AI models can
effectively complement clinical expertise, improving patient stratification and promoting
a more personalized and sustainable approach to lung cancer immunotherapy

## Thesis Context
This repository contains the code and experiments developed for my Master's thesis in Data Science, focused on applying machine learning and deep learning techniques to predict lung cancer patients' responses to immunotherapy.  
The work was conducted in collaboration with Hospital Clínic de Barcelona, within a multidisciplinary research environment combining clinical data analysis and artificial intelligence.
