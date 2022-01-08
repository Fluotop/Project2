# Project2

Analysis of the effect covid19 infection has on cardiomyocytes.
Analysis can be found in the master notebook which will redirect to the DESEQ notebook.

Data
---
Data comes from the following paper: [RNA-Seq of Human iPSC-cardiomyocytes infected with SARS-CoV-2](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE150392)
RNA expression of infected cases were compared to controls. Cases and controls each have three replicates.
The data was downloaded via the SRA identifiers.

Analysis
---
The quality of the reads was checked with FastQC
Reads were then mapped to hg19 reference genome using STAR
Mapped reads were counted using Featurecounts
Difference in gene expression was assessed with DESeq2
Upregulated and downregulated genes were analysed using thid party webtools g:profiler, GOrilla, HumanMine, IRegulon

Conclusion
---
Covid19 infection of cardiomyocytes has a negative effect on the normal function of mitochondria. This makes the hearth have not enough energy to function properly and leads to hearth failure. These results are inline with the paper except that I find no direct evidence for increased apoptosis in cardiomyocytes.
