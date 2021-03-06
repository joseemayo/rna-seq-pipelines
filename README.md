# RNA-seq-Pipelines
Description: RNA-seq Analysis Pipelines

This repository holds the analysis pipelines that I have adapted and used to analyze RNA-seq data from
the following organisms: Arabidopsis thaliana and Homo sapien.

The principal pipeline was adapted from the following nature protocol article: https://www.nature.com/articles/nprot.2016.095
- I was not interested in novel isoforms in this analysis so I used the simplified pipeline described in StringTie's protocol: https://ccb.jhu.edu/software/stringtie/index.shtml?t=manual

Later optimizations were introduced through the referencing of a paper performing a comparison of commonly used RNA-seq tools: https://www.nature.com/articles/s41598-020-76881-x
- Final optimizations included swapping STAR for hisat2 for alignment, having little to no noticable differnce, and using HT-seq to quantify reads in place of StringTie.

Files:

Serial_RNA-seq_Analysis_Pipeline_Prior_to_Optimization.txt
- Original RNA-seq Analysis Pipeline

Serial_RNA-seq_Analysis_Pipeline_Post_Optimization.txt
- Optimized RNA-seq Analysis Pipeline

edgeR_PST_RNA_seq_Analysis_Script.R
- R-script performing basic Differentially Expressed Genes (DEGs) analysis with edgeR using our local dataset.

DESeq2_PST_RNA_seq_Analysis_Script.R
- R-script performing basic Differentially Expressed Genes (DEGs) analysis with DESeq2 using our local dataset.

* This repository will be updated using a working dataset from start to finish using the data from the following publication: https://academic.oup.com/plcell/article/30/6/1199/6099154
