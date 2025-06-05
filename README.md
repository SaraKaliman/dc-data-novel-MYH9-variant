This repository contains code used for the analysis of the Defromability Cytometry experiments done for the project resulting in the publication of the article: "A novel MYH9 variant leads to atypical Epstein-Fechtner syndrome by altering non-muscle myosin IIA mediated contractile processes". The code is written in Jupyter notebooks and it contains following steps:
  1) getting the summary statistics from the raw csv files (mean, median and std for each cell type in the measurement) 
  2) comparing the mechanical cell features (erythrocytes, neutrophils, lymphocytes) of the patients with new MYH9 variant with healthy contols and calculating p-val a effect size for the group comparisson.


Raw csv data comes from DC measurements (rtdc files). Analysis is done acoring to a new standard: U-Net segmentation and unsupervised clustering for selecting the cell types. Details are explained in publications "Small U-Net for fast and reliable segmentation in imaging flow cytometry" and "Automation and Improvement of WBC Mechanical Profiling in Deformability Cytometry".
For this publication rbc_wbc_classifier version v2.0 is used (v2.0) for WBC selection. The code can be found here:
https://gitlab.gwdg.de/sara.kaliman/rbc_wbc_classifier_s3_version/-/tree/v2.0?ref_type=tags
