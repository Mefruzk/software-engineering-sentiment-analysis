# Achieving Reliable Sentiment Analysis in the Software Engineering Domain using BERT (ICSME 2020)

Official implementation of the paper:

> Achieving Reliable Sentiment Analysis in the Software Engineering Domain using BERT  
> IEEE International Conference on Software Maintenance and Evolution (ICSME), 2020.

Primary co-author and repository maintainer: Efruz Karabulut

---

## Overview

This repository contains the experimental implementation used in our ICSME 2020 paper on sentiment analysis for software engineering artifacts.

The approach fine-tunes BERT for domain-specific sentiment classification using 10-fold cross-validation on annotated Stack Overflow data.

---

## Impact

Since its publication in 2020, this work has received over 100 citations and has contributed to advancing sentiment analysis research in software engineering contexts.

## Model

We fine-tune BERT following the methodology described in the paper.  
The original BERT implementation is obtained from:
https://github.com/google-research/bert

---

## Dataset

The dataset consists of annotated software engineering text, including:

- NewData.csv  
- StackOverflow_Original.csv  

Annotation was performed by the co-author Eeshita Biswas.

---

## Reproducibility

### Setup

1. Create Python 3 virtual environment
2. Install dependencies:
   pip install -r requirements.txt
3. Download BERT from the official repository and place under /bert
4. Create:
   - datasets/
   - out/

### Run 10-fold evaluation

python src/tenfold.py --datadir=datasets --out_dir=out

---

## Citation

If you use this repository, please cite:

@inproceedings{biswas2020achieving,
  title={Achieving reliable sentiment analysis in the software engineering domain using bert},
  author={Biswas, Eeshita and Karabulut, Mehmet Efruz and Pollock, Lori and Vijay-Shanker, K},
  booktitle={2020 IEEE International conference on software maintenance and evolution (ICSME)},
  pages={162--173},
  year={2020},
  organization={IEEE}
}
