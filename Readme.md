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

## R Script Workflow

### Step 1: Protein Sequence Retrieval

The human NAAA (N-acylethanolamine-hydrolyzing acid amidase) protein sequence was obtained from the NCBI Protein database using RefSeq accession `NP_055250.2`. The protein corresponds to isoform 1 precursor of *Homo sapiens* and consists of 359 amino acids.

Reference: https://www.ncbi.nlm.nih.gov/protein/NP_055250.2/

### Step 2: Sequence Processing

The protein sequence was retrieved in FASTA format using the `rentrez` package in R. The amino acid sequence was extracted and processed as a series of one-letter amino acid codes for further analysis.

### Step 3: Amino Acid Composition

The NAAA protein sequence was analyzed to determine the frequency and percentage of each of the 20 standard amino acids. The analysis was used to identify the most abundant amino acid residues in the protein.

The five most abundant amino acids identified in the analysis are shown below.

| Amino Acid | Count | Percentage |
|---|---:|---:|
| Leucine (L) | 40 | 11.14% |
| Alanine (A) | 32 | 8.91% |
| Valine (V) | 29 | 8.08% |
| Arginine (R) | 26 | 7.24% |
| Glycine (G) | 25 | 6.96% |

Leucine (L) was the most abundant amino acid among the five listed, accounting for 11.14% of the 359-amino-acid NAAA precursor sequence. Alanine, valine, arginine, and glycine were the next most abundant residues in the reported results.


### Step 5: Data Visualization

Two figures were generated to visualize the results of the NAAA protein sequence analysis:

1. **Amino Acid Composition Bar Plot:** Displays the frequency of each of the 20 standard amino acids in the human NAAA protein sequence and highlights the most abundant residues.
2. **Distribution of Potential N-Linked Glycosylation Motifs:** Illustrates the positions of potential N-linked glycosylation motifs identified using the consensus sequence `N-X-S/T`, where X is any amino acid except proline.

### Step 6: Results and Publication

The analysis outputs were organized into appropriate folders for data, results, and figures. The R script, generated output files, and README documentation were uploaded to GitHub to provide a record of the workflow, methods, and findings of the NAAA protein sequence analysis.

---
## Results and Figure Interpretations

### Figure 1: Amino Acid Composition
<img width="2400" height="1350" alt="NAAA_amino_acid_composition" src="https://github.com/user-attachments/assets/dd07c477-b143-4ba9-b89e-c367aefeafd6" />

**Figure 1.** Distribution of amino acid residues in the NAAA protein sequence.


## Results and Discussion

The analysis of the human NAAA (N-acylethanolamine-hydrolyzing acid amidase) protein, using RefSeq accession `NP_055250.2`, identified a protein sequence containing **359 amino acids**.

### Amino Acid Composition

The five most abundant amino acid residues identified in the NAAA protein sequence are presented below.

| Amino Acid | One-Letter Code | Count | Percentage |
|---|---|---:|---:|
| Leucine | L | 40 | 11.14% |
| Alanine | A | 32 | 8.91% |
| Valine | V | 29 | 8.08% |
| Arginine | R | 26 | 7.24% |
| Glycine | G | 25 | 6.96% |

Leucine was the most abundant residue among those listed, followed by alanine and valine. Leucine and valine are hydrophobic amino acids that may contribute to hydrophobic interactions and protein folding. Alanine can contribute to structural stability, while glycine, because of its small side chain, can provide flexibility in certain regions of a protein.

### Data Visualization and Interpretation

The amino acid composition bar plot illustrates the frequency of amino acid residues throughout the NAAA protein sequence. This visualization helps identify the most common amino acids and compare their relative abundance.

However, amino acid composition alone cannot establish the protein's three-dimensional structure or confirm its enzymatic activity. Additional structural and functional analyses would be needed to investigate these properties.

### Figure 2: Potential N-Linked Glycosylation Motifs
<img width="2400" height="990" alt="NAAA_potential_N_glycosylation" src="https://github.com/user-attachments/assets/ef743c91-06f7-4ab6-8bc2-ec1c609fe8bc" />

**Figure 2.** Positions of potential N-linked glycosylation motifs along the NAGLU protein sequence.

### Interpretation

The sequence analysis identified five potential N-linked glycosylation motifs in the human NAAA protein sequence:

| Position | Motif |
|---:|:---:|
| 37 | NVS |
| 107 | NLS |
| 309 | NAT |
| 315 | NLS |
| 333 | NFT |

These motifs are distributed across different regions of the NAAA protein sequence. Some are located relatively close to one another, particularly in the region around amino acids 309–333. This pattern identifies possible sites for N-linked glycosylation that may warrant further investigation.

N-linked glycosylation can contribute to protein folding, stability, quality control, and intracellular transport. In many lysosomal enzymes, N-linked oligosaccharides can also be modified with mannose-6-phosphate, which helps direct proteins to lysosomes.

**Important limitation:** The consensus sequence `N-X-S/T`, where X is any amino acid except proline, indicates a potential N-linked glycosylation site but does not confirm that glycosylation occurs or that mannose-6-phosphate is present. Sequence analysis alone also cannot establish the enzyme's activity or confirm the biological role of individual motifs.

---

## Questions and Answers

### 1. What does your enzyme normally break down inside lysosomes?

NAAA (N-acylethanolamine-hydrolyzing acid amidase) is a lysosomal enzyme that breaks down N-acylethanolamines, particularly palmitoylethanolamide (PEA), into fatty acids and ethanolamine. This process helps regulate lipid signaling and inflammatory responses in cells.

### 2. What is the total length of your protein, and which amino acids are most common?

The human NAAA protein precursor (RefSeq: `NP_055250.2`) contains **359 amino acids**. Based on the amino acid composition results, leucine (L) is the most abundant residue, with 40 occurrences (11.14%), followed by alanine (A) with 32 (8.91%), valine (V) with 29 (8.08%), arginine (R) with 26 (7.24%), and glycine (G) with 25 (6.96%).

### 3. How many potential N-glycosylation motifs did you find? Where are they located?

The analysis table lists **five potential N-linked glycosylation motifs** in the NAAA protein sequence:

| Position | Motif |
|---:|:---:|
| 37 | NVS |
| 107 | NLS |
| 309 | NAT |
| 315 | NLS |
| 333 | NFT |

These motifs occur at different positions, with three located in the C-terminal region between amino acids 309 and 333. They represent possible glycosylation sites and should be verified against the actual sequence-analysis output.

### 4. Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?

Glycosylation can help lysosomal proteins fold correctly, maintain stability, and move through the cell's protein-processing and transport pathways. In many lysosomal enzymes, mannose-6-phosphate modifications help direct proteins to lysosomes. However, identifying an `N-X-S/T` motif does not prove that the site is glycosylated. Experimental evidence is needed to confirm glycosylation and determine whether a specific modification is present.

### 5. What could happen in the cell if your enzyme did not work properly?

If NAAA does not function properly, the breakdown of N-acylethanolamines, including palmitoylethanolamide (PEA), may be reduced. This could alter lipid signaling pathways involved in inflammation and cellular regulation. The consequences would depend on the extent of enzyme dysfunction, the cell type, and the biological context. Unlike enzymes responsible for degrading major lysosomal storage materials, NAAA primarily regulates bioactive lipid molecules.

## Evidence Screenshots

Uploaded screenshots demonstrating individual work into the `evidence/` folder.

### R Script

<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/a398dea6-689f-46db-b307-0e67ca38aed1" />

### Sequence Analysis
<img width="897" height="306" alt="image" src="https://github.com/user-attachments/assets/8203d65a-4632-4db7-9e19-ae34a28bc99c" />

### Generated Figures

<img width="2400" height="1350" alt="NAAA_amino_acid_composition" src="https://github.com/user-attachments/assets/5d26e29a-1a0a-4974-9857-ad01efb9ffcc" />

<img width="2400" height="990" alt="NAAA_potential_N_glycosylation" src="https://github.com/user-attachments/assets/c18e01e5-a621-4843-91f6-67e3897f2562" />

---

## References
 **NCBI Protein Database:** Human NAAA reference protein record.  
 [  https://www.ncbi.nlm.nih.gov/protein/NP_000254.2](https://www.ncbi.nlm.nih.gov/protein/NP_055250.2/)

