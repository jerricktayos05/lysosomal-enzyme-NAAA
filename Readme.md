# Exploring Lysosomal Enzymes Using NCBI and R: HYAL1

**Name:** Jerrick Paul T. Tayos   
**Section:** B  
**Course/Subject:** BS Biology – Cell and Molecular Biology  
**Selected Gene:** NAAA 

**Enzyme Name:** N-acylethanolamine-hydrolyzing acid amidase isoform 1 precursor

**Organism:** *Homo sapiens* (Human)  

**NCBI RefSeq Protein Accession:** NP_055250.2

---


## Enzyme and Gene Information

- **Gene symbol:** NAAA
- **Enzyme name:** N-acylethanolamine-hydrolyzing acid amidase isoform 1 precursor
- **Organism:** *Homo sapiens* (human)
- **NCBI Protein Accession:** NP_055250.2
- **NCBI Protein Record:** [https://www.ncbi.nlm.nih.gov/protein/NP_695013.1](https://www.ncbi.nlm.nih.gov/protein/NP_055250.2/)

NAAA encodes N-acylethanolamine acid amidase, a lysosomal enzyme that degrades N-acylethanolamines (primarily palmitoylethanolamide), a class of bioactive lipid signaling molecules. This breakdown helps the regulation of lipid amide signaling, anti-inflammatory responses, and pain modulation.

## Objective

The objective of this activity is to analyze the human NAAA lysosomal enzyme by fetching its protein record from NCBI, using R to compute amino acid frequencies and map N-glycosylation motifs, visualizing the data through generated figures, and publishing the complete workflow on GitHub.

## Methods and Workflow

Step 1. Retrieve the NAAA protein sequence from NCBI
The human NAAA (N-acylethanolamine-hydrolyzing acid amidase) protein sequence was selected from the NCBI Protein database using RefSeq accession NP_055250.2. This protein is the isoform 1 precursor of NAAA in Homo sapiens and consists of 359 amino acids. The R script uses the rentrez package to retrieve the protein sequence in FASTA format.

**Code excerpt:**

