# Simplets: Functional Geometry of Protein-Protein Interaction Networks

A tool for analyzing the functional geometry of protein-protein interaction networks using simplicial complexes.

## Authors

- Noel Malod-Dognin
- Natasa Przulj

**Corresponding Author:** Prof. Natasa Przulj  
📧 natasa.przulj@mbzuai.ac.ae

## Overview

Simplets provides a method for characterizing protein-protein interaction networks by analyzing their simplicial complex structure. This approach captures higher-order organizational patterns beyond pairwise interactions.

**Paper:** "Functional Geometry of Protein-Protein Interaction Networks"

## Datasets

Three datasets are provided:

1. **[Dataset 1: Higher-order Interactome Simplicial Complexes](http://www0.cs.ucl.ac.uk/staff/natasa/Simplets/Datasets_Interactomes.7z)** - Biological protein interaction networks
2. **[Dataset 2: Real-world Simplicial Complexes](http://www0.cs.ucl.ac.uk/staff/natasa/Simplets/Datasets_Real.7z)** - Additional real-world networks
3. **[Dataset 3: Random Model Simplicial Complexes](http://www0.cs.ucl.ac.uk/staff/natasa/Simplets/Datasets_Models.7z)** - Null model networks for comparison

*Note: If download links don't work when clicked, copy and paste the URLs directly into your browser's address bar.*

## Installation

### Compile the Code

```bash
git clone https://github.com/przulj-lab/simplets.git
cd simplets

# Compile with optimization
g++ -o SCounter.exe -Wall Simplets.cpp -O3
```

## Usage

```bash
./SCounter.exe <input_simplicial_complex> <output_SDV_file>
```

### Parameters

- `input_simplicial_complex` - Input file containing the simplicial complex
- `output_SDV_file` - Output file for Simplet Degree Vector (SDV)

### Example

```bash
./SCounter.exe protein_network.txt protein_network_SDV.txt
```

## Input Format

The input file should contain the simplicial complex representation of your network.

## Output Format

The output SDV (Simplet Degree Vector) file contains the simplet signatures for analyzing the functional geometry of the network.

## Quick Start

```bash
# 1. Clone and compile
git clone https://github.com/przulj-lab/simplets.git
cd simplets
g++ -o SCounter.exe -Wall Simplets.cpp -O3

# 2. Download datasets
# Download Dataset 1, 2, or 3 from the links above

# 3. Run analysis
./SCounter.exe dataset1/network1.txt output/network1_SDV.txt
```
## Citation

If you use this code or data in your research, please cite:

```
Noel Malod-Dognin and Natasa Przulj
Functional Geometry of Protein-Protein Interaction Networks
 Bioinformatics, Volume 35, Issue 19, October 2019, Pages 3727–3734,
https://doi.org/10.1093/bioinformatics/btz146

```

## Contact

For questions or issues, please contact Prof. Natasa Przulj at natasa.przulj@mbzuai.ac.ae
