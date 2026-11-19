# hemaglobin-beta-comparison-project

Harrison Eilers 

## Project question
How similar are hemoglobin beta protein sequences across humans,
chimpanzees, cows, sheep, and chickens? Which amino acid positions
are identical across these animals?

## Data
I downloaded five protein sequences from UniProt:
- Human: P68871
- Chimpanzee: P68873
- Cow: P02070
- Sheep: P02075
- Chicken: P02112

## Analysis
I aligned the sequences with Clustal Omega and used Python to
calculate percent identity for all 10 animal pairs. Positions
with a gap in either sequence were excluded from each comparison.

I also compared identical positions among the four mammals and
all five animals, using the same 145 gap-free positions.

## Main results
- Human and chimpanzee: 100% identity
- Cow and sheep: 93.10% identity
- Four mammals: 116 of 145 positions conserved (80%)
- All five animals: 86 of 145 positions conserved (59.31%)

## Project files
- Analysis notebook 
- data/: original FASTA files, alignment, and result tables
- figures/: similarity heatmap and conservation chart
- software_versions.txt: software versions used
- ai_usage.md: AI assistance and verification

## How to run
Open the notebook in Google Colab and run the cells. 
The first cell installs the tools and the second downloads the data.


## Software
Python 3.13.18, Biopython 1.88, Pandas 2.2.3,
Matplotlib 3.10.0, Seaborn 0.13.2, Requests 2.32.4,
and Clustal Omega 1.2.4.
