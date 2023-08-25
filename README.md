# MIBC-Bioinformatics
RMarkdown (RMD) File contains code to import quants information from Salmon and then conduct Differential Expression of the Plasma and Urine samples (using DESeq2) in order to identify the statistically significant differentially expressed genes within these groups, as well as amongst each other (all comparison).
The RMD also contains the assorted heatmaps and T-SNE for the samples of this project. The heatmaps show expression within the samples in gene subsets relevant to the comparisons or context of the project. Ex: COSMIC Bladder Cancer Genes, Differentially Expressed genes in plasma invasive vs plasma noninvasive comparisons

The Python file contains the Random Forest model and SHAPley plots used to attempt classification of the urine samples into invasive and noninvasive classes based on a subset of genes (the differentially expressed urine genes identified in the RMD analysis). The model was refined using a GridSearch in the scikit-learn library to find ideal parameters, which allowed for achieving 100% accuracy in classifying the urine samples on a small sample population. The genes used to classify in the model were analyzed using SHAPley values to identify ideal gene candidates. These gene candidates were plotted via heatmap in the RMD once again and were exported for enrichment analysis.
