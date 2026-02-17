# Omics CLI Cheatsheet  
Essential Command-Line Tools for Genome Assembly Workflows

This repository contains commonly used command-line operations in omics workflows.

The commands are intended for use on **Linux** or **HPC** environments and can be adapted for different datasets (FASTQ/FASTA files, read lists, annotation tables, etc.).

## Tools Covered

- **grep** – search for patterns in text files  
- **sed** – stream editor for text replacement  
- **awk** – advanced text processing and filtering  
- **cat** – concatenating and merging files  
- **sort** and **uniq** – sorting and removing duplicates  
- **seqtk** – FASTA/FASTQ manipulation
- **samtools** – SAM/BAM file handling for alignments

These lightweight, widely available tools are extremely useful for preprocessing sequencing data, cleaning files, filtering sequences, renaming headers, subsampling reads, and preparing input for genome assemblers.

## Quick Installation Notes

Most tools are already available on HPC clusters (via `module load` or system packages).  
For seqtk (the only non-standard tool here):

```bash
# Via conda (recommended)
conda install -c bioconda seqtk

# Or compile from source
git clone https://github.com/lh3/seqtk.git
cd seqtk
make
