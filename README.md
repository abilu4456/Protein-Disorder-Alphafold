# Protein Structure Explorer

Analyzes AlphaFold-predicted protein structures by extracting and visualizing 
per-residue confidence scores (pLDDT), and compares folded vs. disordered proteins.

## What it does
- Downloads AlphaFold DB models by UniProt ID
- Extracts pLDDT scores from the PDB B-factor column
- Computes % of residues in each confidence band (very high/confident/low/very low)
- Finds the longest contiguous disordered region
- Visualizes confidence by residue position (color-coded scatter plot)

## Example
Compares RTCB (a structured RNA ligase) against p27^Kip1 (an intrinsically 
disordered protein)

## Requirements
pip install biopython requests matplotlib numpy

## Usage
Run the notebook cells in order, or adapt `scatterbycolor()` and `disorder()` 
for your own UniProt IDs.