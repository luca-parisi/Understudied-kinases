# Understudied kinases

 This project contains the data and jupyter notebook files for:

"Ma, Renfei, Shangfu Li, Luca Parisi, Wenshuo Li, Hsien-Da Huang, and Tzong-Yi Lee. "Holistic similarity-based prediction of phosphorylation
sites for understudied kinases." 

************************************ Folders ******************************************
******
./0_data   ---  This folder contains five files
../Human K_S data.csv  --- This file contains experimentally verified kinase-specific kinase-substrate pairs
../fused kinase_kinase similarity.csv  --- The fuse Kinase-Kinase similarities.
../negative ST sites.csv  ---   Non-phosphorylation ST sites regarded as negative sites. 
../negative Y sites.csv  ---   Non-phosphorylation Y sites regarded as negative sites. 
../understudied_kinases.csv --- The list of the 116 understudied kinases and their categories

******
./1_features  --- This folder contains the encoded KEGG pathway and PPI (encoded with SDNE) features for human proteins


******
./2_models ---  This folder contains two types of predictive models.
../0_ data processing.ipynb  ---  This file is used to find the list of highly similar kinase to understudied kinases
The selection criteria can be refered to the supplementary table of the paper.

The SVM was leveraged as a first pass and trained on sequence-related data only, and the deep learning-based model (FCNN-LSTM) was used as a second pass.
***************************************************************************************

If you use the content, please cite:
"Ma, Renfei, Shangfu Li, Luca Parisi, Wenshuo Li, Hsien-Da Huang, and Tzong-Yi Lee. "Holistic similarity-based prediction of phosphorylation
sites for understudied kinases." 
