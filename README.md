# Enformer PKLR Sickle Cell Analysis

## Overview
This repository contains the computational analysis comparing predicted regulatory activity of the pyruvate kinase gene (PKLR) between normal individuals and sickle cell patients using the Enformer deep learning model.

## Study Details
- **Gene analysed:** PKLR (Pyruvate Kinase Liver and Red Blood Cell)
- **Location:** Chromosome 1 (chr1:155,170,000-155,366,608)
- **Reference Genome:** hg38
- **Population:** YRI (Yoruba in Ibadan, Nigeria) from 1000 Genomes Project
- **Sample size:** 6 individuals (3 normal, 3 sickle cell group)

## Individuals
| Individual | Group | Sample ID | Variants Applied |
|------------|-------|-----------|-----------------|
| Individual 1 | Normal | NA18486 | 41 |
| Individual 2 | Normal | NA18488 | 86 |
| Individual 3 | Normal | NA18489 | 169 |
| Individual 4 | Sickle Cell | NA18498 | 113 |
| Individual 5 | Sickle Cell | NA18499 | 175 |
| Individual 6 | Sickle Cell | NA18501 | 39 |

## Requirements
- Python 3.8+
- TensorFlow 2.x
- tensorflow-hub
- pyfaidx
- numpy
- matplotlib
- bcftools
- samtools
- tabix

## Data Sources
- Reference genome: UCSC Genome Browser (hg38)
- Variant data: 1000 Genomes Project high coverage phase 3
- Enformer model: DeepMind via TensorFlow Hub

## Key Results
- Maximum Log2 Fold Change: 4.71
- Mean Log2 Fold Change: 0.036
- Enformer output: 896 genomic bins x 5,313 regulatory tracks

## Repository Structure
- notebooks/ — Colab notebook with full analysis code
- results/ — Output plots and figures
- data/ — Input data files

## License
MIT
