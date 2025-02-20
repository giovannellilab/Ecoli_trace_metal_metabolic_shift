# Trace elements availability controls terminal electron acceptor utilization in E. coli

[![forthebadge](https://forthebadge.com/images/badges/cc-by.svg)]([https://forthebadge.com](https://creativecommons.org/licenses/by/4.0/))
[![forthebadge](https://forthebadge.com/images/badges/powered-by-coffee.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-science.svg)](https://forthebadge.com)

[![giovannellilab](https://img.shields.io/badge/BY-Giovannelli_Lab-blue)](https://www.donatogiovannelli.com)
[![funded-by-erc](https://img.shields.io/badge/Funded%20by-ERC-ff6400.svg)](https://erc.europa.eu/homepage)
[![projetc-coevolve](https://img.shields.io/badge/Project-ERC%20CoEvolve-000fa9.svg)](https://www.coevolve.eu/)
[![forged-with-Metals](https://img.shields.io/badge/Forged%20with-Metals-purple.svg)]()
[![made-with-R](https://img.shields.io/badge/Coded%20in-R-red.svg)](https://www.r-project.org/)


Data and code relative to the Ricciardelli et al. 2024 manuscript on the effect of trace metals in controlling the metabolic shifts between alternative electron acceptors in _Escherichia coli_ and other oganisms. 
The _E. coli_ genome is available in NCBI under project PRJEB85325, while the proteomic data are available in the PRoteomics IDEntifications (PRIDE) database (https://www.ebi.ac.uk/pride/) at the European Bioinformatics Institute (EMBL-EBI, Hinxton, Cambridge, UK) with accession number PXD059598.

This repository contains the following files:

- README.md (this readme file)
- GEM-collection_MAGs_annotation.ipynb containing the code for the plotting of the MAGs terminal reductase data
- hmm_moldes folder, containing the hmm profiles used to annotate the MAGs downloaded from [the JGI GEM collection](https://genome.jgi.doe.gov/portal/GEMs/GEMs.home.html). 
- hmm_moldes folder, containing the individual results from the hmmer3 search obtained using the follwing command: ```hmmsearch --cpu 12 --tblout results_table_gene.txt MODEL.hmm.gz GEM_combined_mags.faa.gz > results_gene.log```
- Ecoli_k12_DH5.fna containing the nucleotide fasta file of the _E. coli_ genome
- Ecoli_k12_DH5.gff containign the gff annotation of the _E. coli_ genome
- Ecoli_growth_data.csv containing the growth experiment data for _E. coli_
- Bsubtili_growth_data.csv containing the growth experiment data for _Bacillus subtilis_
- Sbacillaris_growth_data.csv containing the growth experiment data for _Stichococcus bacillaris_
- Sbacillaris_rETR_data.csv containiong the rETR data from S. bacillaris
- IPCMS_metal_data.csv containing the results of the ICP-MS trace metal data
- DE_proteins_proteome folder, contaning the tables of the differentially expressed genes at the 3 time points 

Please cite as:

Annarita Ricciardelli, Benoit de Pins, Jacopo Brusca, Monica Correggia, Luciano Di Iorio, Martina Cascone, Marco Giardina, Stefany Castaldi, Rachele Isticato, Roberta Iacono, Marco Moracci, Nunzia Nappi, Antonino Pollio, Costantino Vetriani, Serena Leone, Angelina Cordone, Donato Giovannelli1. 2025. Trace elements availability controls terminal electron acceptor utilization in Escherichia coli. _BioArXiv_ https://doi.org/10.1101/2025.01.08.631794
