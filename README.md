
## Introduction

This repo holds the source code and scripts for “DESIRE: An Efficient Dynamic Cluster-based Forest Indexing for Similarity Search in Multi-Metric Spaces”

## Usage

1. Datasets

The used datasets has the following files:
	*.txt
	*_q.txt	
The first file contains all the data, and the first line for datasets denotes the size, the dimention.
The second line describe the used metrics (taking 0 as an example, it means L-1 Norm Distance) and the third line provide the maximum distance for each metric.
The second file contains the query parameters and the ids  for the quries.
The first line and the second line decribe the k for knn and the radius for range query.

2. Indexes

We implemented all the indexes using C++ with Visual Studio 2019.
This file contains the source code files for M3-tree, PM-tree, RR*-tree and our DESIRE 
In the sub folder, file 'data' contains the dataset, the query file and the execute parameters. 
When using different dataset, modify the file 'par.txt', where the first parameter is the dataset path and the second is the query file path.


## Compared algorithms

| __Algorithm__ | __Paper__ | __Year__ |
|-------------|------------|------------|
M3-tree | Adapting metric indexes for searching in multi-metric spaces | 2012
PM-tree | Indexing Multi-Metric Data | 2016
RR*-tree | Indexing Multi-Metric Data | 2016


## Datasets

Each dataset can be obtained from the following links, while the synchronized dataset can be generalized following the decriptions in our paper. 

| __Dataset__ | __link__ | __Metrics__ |
|-------------|------------|------------|
| Hornets        |  https://agr.wa.gov/departments/insects-pests-and-weeds/insects/hornets/data  | 4 |
| Rental      | https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries | 5 |
| Food         | https://world.openfoodfacts.org/data | 9 |


Two sample datasets are included in the folder 'Dataset'.

## Citation
If you use our code for research work, please cite our paper as below:
```
@article{,
	author = {Zhu, Yifan and Chen, Lu and Gao, Yunjun and Zheng, Baihua and Wang, Pengfei},
	title = {DESIRE: An Efficient Dynamic Cluster-Based Forest Indexing for Similarity Search in Multi-Metric Spaces},
	year = {2022},
	publisher = {VLDB Endowment},
	volume = {15},
	number = {10},
	issn = {2150-8097},
	journal = {Proc. VLDB Endow.},
	month = {sep},
	pages = {2121–2133},
	numpages = {13}
}
```
