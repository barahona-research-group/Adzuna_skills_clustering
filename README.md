# Skills_clustering
Code and data for [Patterns of co-occurrent skills in UK job adverts](https://arxiv.org/abs/2406.03139)

## Overview

This repository contains two main files:

1. **Jupyter Notebook**: This notebook provides a step-by-step guide on how to process raw JSON files from Adzuna to generate a co-occurrence matrix. The matrix is then used for carrying out the clustering analysis by [PyGenStability](https://github.com/barahona-research-group/PyGenStability.git).
2. **Excel Spreadsheet**: This spreadsheet consists of the two optimal clusterings from the co-occurrence matrix obtained by PyGenStability.

## Repository Contents

### Jupyter Notebook

- **File Name**: `tutorial.ipynb`
- **Description**: This notebook walks you through the process of converting raw JSON data into a co-occurrence matrix. It includes data loading and matrix generation.

#### Key Steps in the Notebook:

1. **Get co-occurrences from raw Adzuna data**: Instructions on how to load and extract skills co-occurrences from raw JSONs after deduplication.
2. **Convert to Pandas dataframe**: Creating a Pandas dataframe in which the columns and rows are skills and the entries are the number of co-occurrences.

### Excel Spreadsheet

- **File Name**: `optimal_clusterings_fulldata.xlsx`
- **Description**: This spreadsheet contains two sheets that consist of the clustering of the skills into 7 clusters and 21 clusters.
- **Columns**: `Lightcast_skills` contains the unique skills in the job adverts. `Cluster` contains the clusters of the skills.

## Cite

Please cite our paper if you use this code in your own work:
```
@article{liu2024patterns,
  title={Patterns of co-occurrent skills in UK job adverts},
  author={Liu, Zhaolu and Clarke, Jonathan and Rohenkolh, Bertha and Barahona, Mauricio},
  publisher = {arXiv},
  year = {2024},
  doi = {10.48550/ARXIV.2406.03139},
  url = {https://arxiv.org/abs/2406.03139}
}
```

---
