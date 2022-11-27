# Holistic similarity-based prediction of phosphorylation sites for understudied kinases

### Description

This repository contains the data and Jupyter notebook files used in the paper mentioned in the `Citation request` 
section below. 
The selection criteria leveraged to identify highly similar kinases with respect to understudied kinases 
are included in the supplementary table of the paper.
The Machine Learning-driven model `SVM` was used as a first pass and trained on sequence-related data only, and 
the Deep Learning-driven model (FCNN-LSTM) was leveraged as a second pass.

### Dependencies

The codes in the Jupyter notebooks (.ipynb files) of this repository were developed in Python 3.9.7.
The following libraries were installed via `pip` and leveraged as follows:
- `keras` for Deep Learning modelling
- `numpy` for handling train, validation, and test data partitions/splits
- `pandas` for dealing with dataframes of inputs and predictive results
- `pickle` for de-serialising feature embeddings
- `sklearn` for splitting the data into train and test partitions, as well as for Machine Learning modelling and assessment of predictive performance
- `statistics` for computing the mean of various predictive performance-related metrics

### Repository structure and usage

```
.
├── 0_data                                     # Folder containing five data-related files
│   ├── fused kinase_kinase similarity.csv        # The fuse Kinase-Kinase similarities
│   ├── Human K_S data.csv                        # Experimentally-verified kinase-specific kinase-substrate pairs
│   ├── negative ST sites.csv                     # Non-phosphorylation ST sites regarded as negative sites
│   ├── negative Y sites.csv                      # Non-phosphorylation Y sites regarded as negative sites
│   └── understudied_kinases.csv                  # List of the 116 understudied kinases and their categories
│
├── 1_features                                 # The encoded KEGG pathway and PPI (encoded with SDNE) features for human proteins
│
├── 2_notebooks                                # Folder containing Jupyter notebook files
│   ├── 0_data_processing.ipynb                   # File used to identify the list of highly similar kinases with respect to understudied kinases
│   ├── 1_SVM_model.ipynb                         # File on the SVM predictive model
│   └── 2_FCNN_LSTM_model.ipynb                   # File on the FCNN-LSTM predictive model
│
├── .gitattributes
├── .gitignore
├── LICENSE
└── README.md
```

### Citation request

If you use these data and/or codes, please cite the following paper currently under review:

- "Renfei Ma, Shangfu Li, Luca Parisi, Wenshuo Li, Hsien-Da Huang, and Tzong-Yi Lee. Holistic similarity-based prediction of phosphorylation
sites for understudied kinases." 
