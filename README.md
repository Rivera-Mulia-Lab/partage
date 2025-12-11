# PARTAGE: Parallel analysis of replication timing and gene expression
The human genome is partitioned into functional compartments that replicate at specific times during the S-phase. This temporal program, referred to as replication timing (RT), is co-regulated with the 3D genome organization, is cell type-specific, and changes during development in coordination with gene expression. Moreover, RT alterations are linked to abnormal gene expression, genome instability, and structural variation in multiple diseases, including cancer. Here, we developed PARTAGE, a multiomics approach that enables joint profiling of copy number variation (CNV), RT, and gene expression from the same sample, providing a more accurate integrative view of the complex relationships between RT and gene regulation. This computational framwork compiles the pipelines to analyze and visualze the distinct modalities of PARTAGE: RT, CNV, and RNA-seq.


<img width="3323" height="1606" alt="Figure1_v1_white" src="https://github.com/user-attachments/assets/74ecb6c3-235a-4136-af82-ca142b5cce9a" />




Scripts for the analysis of PARTAGE data
Consists of four jupyter notebook files, an R script, and two conda env files

PARTAGE_RT.ipynb: Used for calculating and plotting partage data. Requires RPKM data for G1 samples and other timepoints. Will output correlation graph and PARTAGE heatmap representing the replication timing.

rna_enrichment_corr.ipynb: Used for calculating clusters and enrichment analysis of expression data, along with self-correlation and correlation between pseudo-RT and expression.

CNV_Analysis_plot.ipynb: Used for plotting copy number variation along with called deletions and duplications called by CNVpytor. Outputs calls text file for use with ProOvErlap

convert_calls_to_bed.ipynb: convert text file output to bed for ProOvErlap

QuantileNorm_Smoothing_10kb.R: Used for the quantile normalization and loess smoothing of the log2 RT data. Package requirements and usage are listed inside.

partage_data_analysis_environment.yml: YML file containing the packages used for the conda environment for the plotting and analysis of the PARTAGE data

pipeline_environment.yml: YML file containing the packages used for the conda environment for the processing of raw fastq files to RPKM and log2 RT files.
