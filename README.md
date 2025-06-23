Master's Thesis: Multiomic Integration of Monoglyceride Response in Adipose Tissue Macrophages with Obesity

Overview

This repository contains the complete set of analytical scripts, visualizations, and methodological details used for my Master's thesis, which explores the multiomic integration of transcriptomic, lipidomic, and spatial lipidomic data from adipose tissue macrophages treated with monoglycerides. The overarching aim was to characterize biological responses relevant to obesity and metabolic diseases.

Background and Motivation

Obesity and its associated metabolic disorders represent major public health challenges. Adipose tissue macrophages play a critical role in mediating inflammatory and metabolic responses. Investigating the multiomic response of these cells to lipid treatments, particularly monoglycerides, provides valuable insights into mechanisms driving inflammation and lipid metabolism in obesity.

Experimental Details

Cell Model: Adipose tissue macrophages

Treatment Conditions: Monoglyceride (MAG), Oleic Acid (OA), Palmitic Acid (PA)

Concentrations: High dose (5 mM) and low dose (500 µM)

Analysis Approaches:

Transcriptomic analysis via bulk RNA-seq

Lipidomic analysis via LC-MS

Spatial lipidomics via imaging mass spectrometry (IMS)

Project Objectives

Transcriptomic analysis: Identify gene expression profiles and differential expression across lipid treatments.

Lipidomic analysis: Characterize lipid species influenced by monoglyceride treatment.

Spatial lipidomics: Visualize spatial distributions of lipid species within macrophage-rich adipose tissue.

Multiomic integration: Correlate and interpret combined omic datasets to generate novel biological insights.

Repository Contents

Analysis Scripts (.Rmd files)

PCA, Clustering, and Project Overview (PCA + Cluster + Gene Purpose Labeling + Project Schematic Figure.Rmd)

Principal Component Analysis and clustering

Schematic figure of experimental design and multiomic workflow

PCA and Heatmap Visualizations (PCAPlot + Gene Rank Plot + Heatmaps.Rmd)

PCA plots

Gene rank plots highlighting average differential expression (top 25 genes)

Heatmaps illustrating expression patterns for top-ranked genes

Detailed PCA Comparison (PCAPlotsPart2 500uM + 5mM.Rmd)

PCA visualizations specifically comparing 500 µM and 5 mM lipid treatments

Differentially Expressed Genes (Up&DownRegulatedGeneList.Rmd, Up&DownRegulatedPART2.Rmd)

Identification and analysis of significantly upregulated and downregulated genes across treatment conditions

Venn Diagrams and GO Analysis (VennDiagram.Rmd, VennDiagramG5-G8 + GoTerm.Rmd)

Venn diagrams comparing gene overlap across experimental groups

GO enrichment analyses identifying functional biological pathways

Software and Dependencies

R (version 4.2 or newer recommended)

RStudio

Key R packages: DESeq2, ggplot2, pheatmap, clusterProfiler, enrichplot, VennDiagram, tidyverse

To install necessary packages in R, run:

packages <- c("DESeq2", "ggplot2", "pheatmap", "clusterProfiler", "enrichplot", "VennDiagram", "tidyverse")
install.packages(setdiff(packages, rownames(installed.packages())))

Instructions to Reproduce Analysis

Clone or download this repository to your local environment.

Open .Rmd files in RStudio.

Ensure required packages (listed above) are installed.

Execute code blocks sequentially as described within each RMarkdown document.

Key Findings

Differentially expressed genes and lipid species were identified, providing insights into lipid metabolism and inflammatory pathways in obesity.

Spatial lipidomics revealed specific lipid accumulation around macrophage-rich areas, suggesting targeted inflammatory responses.

Multiomic integration uncovered potential mechanistic links between lipid treatments and macrophage metabolic activity.

Troubleshooting and Tips

Ensure package versions are consistent to avoid compatibility issues.

Data paths may need adjustments depending on your local setup; clearly defined working directories are recommended.

Figures and Results

Figures generated through scripts include PCA plots, heatmaps, schematic figures, and Venn diagrams. These visual outputs provide detailed insight into data relationships and biological implications.

Contact and Citation

For any questions regarding this repository or the associated analyses, please reach out directly or via GitHub issues. To cite this work, please reference:

Trindade, Gui. (2025). Multiomic Integration of Monoglyceride Response in Model Adipose Tissue Macrophages with Obesity. Master's Thesis, NYU.
