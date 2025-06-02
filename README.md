This repository contains code used for the analysis of the Defromability Cytometry experiments done for the project resulting in the publication of the article: "A novel MYH9 variant leads to atypical Epstein-Fechtner syndrome by altering non-muscle myosin IIA mediated contractile processes". The code is written in Jupyter notebooks and it contains following steps:
  1) getting the summary statistics from the raw csv files (mean, median and std for each cell type in the measurement) 
  2) comparing the mechanical cell features (erythrocytes, neutrophils, lymphocytes) of the patients with new MYH9 variant with healthy contols and calculating p-val a effect size for the group comparisson.


Raw csv data comes from rtdc files. Cell types were selected using algorithm explained in the publication "Automation and Improvement of WBC Mechanical Profiling in Deformability Cytometry".
For this publication an older version of that algorithm is used (v2.0) to select neutrophils and lymphocytes. The code for the algorithm used to produce raw data can be found here:
https://gitlab.gwdg.de/sara.kaliman/rbc_wbc_classifier_s3_version/-/tree/v2.0?ref_type=tags
