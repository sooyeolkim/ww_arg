# Overview
This github contains collection of codes used for manuscript Wastewater surveillance reveals patterns of antibiotic resistance across the United States by Kim, Zulli, Chan, Duong, Linfield, McCormack, White, Wolfe, Boehm, and Pickering. The R markdown files contain text and comments to help guide readers through the code. R version 4.3.0 was used. All packages used in the code are indicated in each file. 

## Brief description of the files
* ww_arg.Rmd: This code takes input files of raw dPCR data and goes through QA/QC and merges it with the secondary data. The output files are dPCR data that's gone through QA/QC, averaged dPCR data across time points (which we consider to be replicates in this study), dPCR data merged wtih secondary datasets with/without outliers, antibiotic resistance gene (ARG) concentration expressed as prevalence in terms of z-score, and ARG prevalence in terms of sum of concentrations. The output file was aggregated and organized for readability and posted in the Stanford Data repository (address below). The original data files (with the exception of antibiotic prescription data, which is proprietary and could not be shared publicly) can be requested through the author. This code should not take more than a few minutes to run. 
* ww_arg_3.Rmd: This code takes the output of ww_arg and runs correlational analysis. The main outputs are figures and results of statistical tests. This code also should not take more than a few minutes to run. 
* ww_arg_RF.Rmd: This code runs the random forest prediction model. The main outputs are prediction maps and results of the random forest modeling. This code should not take more than an hour to run.

## Notes 
All data used for analysis are available on the Stanford Data Repository: https://purl.stanford.edu/vb318cm9509. The antibiotic prescription data from Epic Cosmos could not be made publicly available and therefore are excluded. 
