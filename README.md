This repository contains code used for the analysis of the Deformability Cytometry (DC) measurements from the publication of the article: "A novel MYH9 variant leads to atypical Epstein-Fechtner syndrome by altering non-muscle myosin IIA mediated contractile processes".
The code is written in Jupyter notebooks and it contains following steps:
  1) getting the summary statistics from the raw csv files (mean, median and std for each cell type in the measurement) 
  2) comparing the mechanical cell features (erythrocytes, neutrophils, lymphocytes) of the patients with new MYH9 variant with healthy controls. Code produces main figure in the article as well as the t-test p-val and Cohen´s effect size for the group comparison.


csv datasets can be found here: https://dcor.mpl.mpg.de/group/myh9_data

Csv data comes from DC measurements that are recorded as rtdc files (hdf5 format). These files contain brightfield images of all blood cells. Cell features are extracted by first segmenting the images using small U-Net followed by selection of wbc types using filters and unsupervised clustering and selection of focused rbc using filters. Details of this standard analysis pipeline are explained in publications "Small U-Net for fast and reliable segmentation in imaging flow cytometry" and "Automation and Improvement of WBC Mechanical Profiling in Deformability Cytometry".
In this publication rbc_wbc_classifier version v2.0 is used for WBC selection. The code can be found here: https://gitlab.gwdg.de/sara.kaliman/rbc_wbc_classifier_s3_version/-/tree/v2.0?ref_type=tags
