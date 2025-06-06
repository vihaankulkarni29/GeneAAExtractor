# GeneAAExtractor

# 🧬 GeneAAExtractor

GeneAAExtractor is a lightweight Google Colab tool for extracting amino acid sequences of specific genes directly from GFF3 and FASTA files. It's designed for microbiologists, bioinformaticians, and AMR researchers working with genome annotations and isolate analysis.

## 🚀 Features
- Extracts amino acid sequences for only the user-specified genes
- Works with `.gff3`, `.fasta`, and `.txt` gene list inputs
- Supports strand orientation and reverse complement logic
- Exports individual `.faa` files for each gene in the format: `GeneName IsolateName.faa`
- Automatically zips all extracted protein files for download

## 📂 Input Files
1. **GFF3 file** – Genome annotations
2. **FASTA file** – Genomic sequence
3. **TXT file** – List of gene names to extract (one per line, case-sensitive optional)

## 🧪 Output
A `.zip` archive containing one `.faa` file per gene:
acrA SSS08.faa
blaTEM SSS08.faa
dfrA12 SSS08.faa


## 🛠 How to Use
1. Open the tool in **Google Colab**
2. Upload your `.gff3`, `.fasta`, and `.txt` files
3. Enter your isolate name when prompted
4. The tool processes your genome and downloads the protein `.zip`

## 👩‍🔬 Example Use Case
```bash
Input:
  - ecoli_annotations.gff3
  - ecoli_genome.fasta
  - gene_list.txt (contains: acrA, acrB, blaTEM)

Output:
  - acrA SSS08.faa
  - acrB SSS08.faa
  - blaTEM SSS08.faa

📦 Dependencies
Python 3.7+

Biopython

📄 License
MIT License – free to use and adapt for academic or research purposes.

✨ Acknowledgements
Developed with love for wet-lab researchers looking to automate their isolate curation workflows.
