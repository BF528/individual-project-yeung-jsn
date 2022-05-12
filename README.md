# Project Description

This project conducts analyses described in the Data Curator and Programmer roles for Project 3 (Concordance of microarray and RNA-Seq differential gene expression). All data processing and analysis was performed on BU's Shared Computing Cluster.


The datasets used in this project were presented in:

Wang et al. A comprehensive study design reveals treatment- and transcript abundance–dependent concordance between RNA-seq and microarray data. Nature Biotechnology. 2014.

## Repository Contents
---
### Data Curator

fastqc.qsub
- qsub script runs FastQC on fastq files

STAR.qsub
- qsub script runs STAR align against rat genome

multiqc.qsub
- qsub script to compile STAR and FastQC outputs

---

### Programmer

featureCounts.qsub
- qsub script performs featureCount mapping of reads to gene features

featureCounts_multiqc_qsub
- qsub script compiles featureCounts outputs

preprocessing.Rmd
- compiles count data for all samples into single count matrix

deseq.Rmd
- performs differential expression analysis and visualization of deseq results

---
