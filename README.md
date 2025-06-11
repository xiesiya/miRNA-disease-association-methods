# 🏎💨From Biogenesis to Algorithms: A Holistic Review of miRNA-Disease Prediction Computational Methods with Experimental Benchmarking
<a href='https://github.com/xiesiya/miRNA-disease-association-methods/blob/main/README.md'></a>
![GitHub stars](https://img.shields.io/github/stars/xiesiya/miRNA-disease-association-methods?color=red) 
![GitHub forks](https://img.shields.io/github/forks/xiesiya/miRNA-disease-association-methods?color=green&label=Fork)

<p align="center"> 
  Visitor count<br>
  <img src="https://profile-counter.glitch.me/xiesiya.miRNA-disease-association-methods/count.svg" />
</p>


## What is miRNA?
RNA can be divided into two categories based on its coding function: (1) RNAs with coding potential, and (2) RNAs without coding potential, also known as non-coding RNA (ncRNA), which includes microRNAs (miRNA), snoRNAs, circRNAs and lncRNAs. Long non-coding RNAs (lncRNAs) are a major class of important ncRNAs with the lengths more than 200 nucleotides. An increasing number of lncRNA have been found to be abnormally expressed in human diseases, and play a critical role in tumor development.

  
## Overview
* We collect miRNA- and disease-related databases for MDA prediction, including miRNA-disease association databases, miRNA-related databases, and disease-related databases. 
* We provide the first a comprehensive overview of 67 MDA prediction methods, classify them into five categories, as shown below figure 1.
![classification](https://github.com/user-attachments/assets/4e4202c0-43dd-49dc-8951-9763aaa6ee20)
Fig 1: Classification of computational methods for MDA prediction. 

## **Data resources**

### **miRNA-disease association data resources**

| Database | Description | URL |
| --- | --- | --- |
| HMDD v3.2 | Collects 35547 experimentally confirmed MDAs, involving 1206 miRNA genes and 893 diseases | http://www.cuilab.cn/hmdd |
| dbDEMC 3.0 | Contains 3268 differentially expressed miRNAs for 40 cancer types from humans, mics, and rats | https://www.biosino.org/dbDEMC |
| miR2Disease | Records 349 miRNAs, 163 diseases, and 3273 entries | http://www.mir2disease.org/ |
| miRCancer | Provides 9080 associations between 196 human cancers and 57984 miRNAs | http://mircancer.ecu.edu/ |
| miRwayD | Collects 663 miRNA-pathway association entries for 76 diseases, involving 232 miRNAs, 122 pathways, and 328 targeted genes | http://www.mirway.iitkgp.ac.in/ |
| MNDR (RNADisease v4.0) | Stores 343,273 associations between more than 18 RNA categories, 117 species, and 4090 diseases | http://www.rnadisease.org/ |

### **miRNA-related data resources**

| Database | Description | URL |
| --- | --- | --- |
| miRbase v22 | Responsible for miRNA naming and is the primary public repository for miRNA sequences and annotations | https://www.mirbase.org/ |
| mirTarbase | Stores experimentally verified miRNA-target interactions. containing 19912394 interactions between 4630 miRNAs and 27172 mRNAs (target genes) | [https://miRTarBase.cuhk.edu.cn/](https://mirtarbase.cuhk.edu.cn/) |
| miRWalk | Provides experimentally verified miRNA-gene interactions | http://mirwalk.umm.uni-heidelberg.de/ |
| starbase (ENCORI) | Collects regulatory relationships on miRNA-ceRNA, miRNA-ncRNA, and protein-RNA interaction | https://starbase.sysu.edu.cn/ |
| lncRNASNP2 | Contains experimentally verified miRNA-lncRNA interactions | http://bioinfo.life.hust.edu.cn/lncRNASNP |
| miREnvironment | Records experimentally supported interactions between miRNAs, environmental factors, and phenotypes | http://www.cuilab.cn/miren |

### **Disease-related data resources**

| Database | Description | URL |
| --- | --- | --- |
| MeSH | Is the NLM controlled vocabulary thesaurus used for indexing, cataloging, and searching of biomedical and health-related information | http://www.nlm.nih.gov/ |
| HPO | Offers a comprehensive logical standard to depict and computationally analyze phenotypic abnormalities within human disease | https://hpo.jax.org/app/ |
| OMIM | Records collated information about genes and genetic phenotypes and the relations between them, with 26,588 entries covering 7,248 diseases and 4,685 genes | http://www.ncbi.nlm.nih.gov/omim |
| DisGeNet | Contains publicly available collections of genes and variants related to human diseases | https://www.disgenet.org/ |
| LncRNADisease | Provides experimentally verified and predicted lncRNA-disease associations and circRNA-disease associations, as well as regulatory relationships between lncRNAs, mRNAs, and miRNAs | http://www.rnanut.net/lncrnadisease/ |

## Classical Computational models for predicting MDAs

- **Network-based Methods**
    
    ### **Random walk**
    
    1. 【**MIDP (**Xuan et al., **2015)**】Xuan P, Han K, Guo Y, et al. Prediction of potential disease-associated microRNAs based on random walk[J]. Bioinformatics, 2015, 31(11): 1805-1815.      [[Download]](https://academic.oup.com/bioinformatics/article/31/11/1805/2364959)   [[Code]](http://bioinfolab.stx.hk/midp/)
    2. 【**IFMDA (**Liu et al., **2016)**】Liu Y, Zeng X, He Z, et al. Inferring microRNA-disease associations by random walk on a heterogeneous network with multiple data sources[J]. IEEE/ACM transactions on computational biology and bioinformatics, 2016, 14(4): 905-915.  [[Download]](https://ieeexplore.ieee.org/abstract/document/7447729)   [[Code]](http://ifmda.aliapp.com) 
    3. 【**BRWH (**Luo et al., **2017)**】Luo J, Xiao Q. A novel approach for predicting microRNA-disease associations by unbalanced bi-random walk on heterogeneous network[J]. Journal of biomedical informatics, 2017, 66: 194-203.      [[Download]](https://www.sciencedirect.com/science/article/pii/S1532046417300084#ab015)   [[Code]](https://github.com/xxpaaa/PATMDA)  
    4. **【BRWHNHA (**Yu et al., **2019)**】Yu D L, Ma Y L, Yu Z G. Inferring microRNA-disease association by hybrid recommendation algorithm and unbalanced bi-random walk on heterogeneous network[J]. Scientific reports, 2019, 9(1): 2474.    [[Download]](https://www.nature.com/articles/s41598-019-39226-x)   [[Code]](https://github.com/myl446/BRWHNHA)  
    5. 【**RWBRMDA (**Niu et al., **2019)**】Niu Y W, Wang G H, Yan G Y, et al. Integrating random walk and binary regression to identify novel miRNA-disease association[J]. BMC bioinformatics, 2019, 20: 1-13.     [[Download]](https://link.springer.com/article/10.1186/s12859-019-2640-9) 
    6. 【**RWRMMDA (**Nguyen et al., **2021)**】Nguyen V T, Le T T K, Than K, et al. Predicting miRNA–disease associations using improved random walk with restart and integrating multiple similarities[J]. Scientific Reports, 2021, 11(1): 21071.      [[Download]](https://www.nature.com/articles/s41598-021-00677-w#Sec2)
    7. 【**BRWRMHMDA** (Qu et al., 2021)】Qu, Jia, et al. "Biased random walk with restart on multilayer heterogeneous networks for MiRNA–disease association prediction." ***Frontiers in Genetics*** 12 (2021): 720327.     [[Download]](https://www.frontiersin.org/journals/genetics/articles/10.3389/fgene.2021.720327/full) 
    8. 【**PATMDA  (**Xie et al., **2023)**】Xie X, Wang Y, He K, et al. Predicting miRNA-disease associations based on PPMI and attention network[J]. BMC bioinformatics, 2023, 24(1): 113.    [[Download]](https://link.springer.com/article/10.1186/s12859-023-05152-z)   [[Code](https://github.com/xxpaaa/PATMDA)
    9. 【**SLMRWMDA (**Yao et al., **2024)**】Yao H, Hou Z, Zhang W, et al. Prediction of microRNA-disease potential association based on **sparse learning and multilayer random walks**[J]. Journal of Computational Biology, 2024, 31(3): 241-256.     [[Download]](https://www.liebertpub.com/doi/abs/10.1089/cmb.2023.0266)
    10. 【**HGTMDA   (**Lu et al., **2024)**】Lu D, Li J, Zheng C, et al. HGTMDA: A Hypergraph Learning Approach with Improved GCN-Transformer for miRNA–Disease Association Prediction[J]. Bioengineering, 2024, 11(7): 680.  [[Download]](https://www.mdpi.com/2306-5354/11/7/680)  
    11. 【**AE-RW (**Lu et al., **2024)**】Lu P, Jiang J. AE-RW: Predicting miRNA-disease associations by using autoencoder and random walk on miRNA-gene-disease heterogeneous network[J]. Computational Biology and Chemistry, 2024, 110: 108085.    [[Download]](https://www.sciencedirect.com/science/article/pii/S1476927124000732) 
    
    ### **Others**
    
    1. 【**WBSMDA (**Chen et al., **2016)**】Chen X, Yan C C, Zhang X, et al. WBSMDA: within and between score for MiRNA-disease association prediction[J]. Scientific reports, 2016, 6(1): 21106.  [**[Download]](https://www.nature.com/articles/srep21106#Sec2)** 
    2. 【**PBMDA (**You et al., **2017)**】You Z H, Huang Z A, Zhu Z, et al. PBMDA: A novel and effective path-based computational model for miRNA-disease association prediction[J]. PLoS computational biology, 2017, 13(3): e1005455.  [**[Download]](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005455#sec011)** 
- **Matrix Factorization-based Methods**
    1. 【**GRNMF (**Xiao et al., **2018)**】Xiao Q, Luo J, Liang C, et al. A graph regularized non-negative matrix factorization method for identifying microRNA-disease associations[J]. Bioinformatics, 2018, 34(2): 239-248.    **[[Download]](https://academic.oup.com/bioinformatics/article-abstract/34/2/239/4101940)   [[Code]](https://github.com/XIAO-HN/GRNMF/)**  
    2. 【**IMCMDA (**Chen et al., **2018)** 】Chen X, Wang L, Qu J, et al. Predicting miRNA–disease association based on inductive matrix completion[J]. Bioinformatics, 2018, 34(24): 4256-4265.  [**[Download]](https://academic.oup.com/bioinformatics/article/34/24/4256/5043011?login=false)**  [**[Code]**](https://github.com/lazywolf007/IMCMDA)
    3. 【**MDHGI (**Chen et al., **2018)**】Chen X, Yin J, Qu J, et al. MDHGI: matrix decomposition and heterogeneous graph inference for miRNA-disease association prediction[J]. PLoS computational biology, 2018, 14(8): e1006418.   [**[Download]](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006418#sec010)**  [**[Code]**](https://github.com/wengelearning/MDHGI)
    4. 【**NMFMC (**Zheng et al., **2022)**】Zheng X, Zhang C, Wan C. MiRNA-Disease association prediction via non-negative matrix factorization based matrix completion[J]. Signal Processing, 2022, 190: 108312.   [**[Download]](https://www.sciencedirect.com/science/article/abs/pii/S0165168421003492)**  [**[Code]**](https://git.l3s.uni-hannover.de/dong/simplifying_mirna_disease)
    5. 【**WeightTDAIGN (**Ouyang et al., **2022)**】Ouyang D, Miao R, Wang J, et al. Predicting multiple types of associations between miRNAs and diseases based on graph regularized weighted tensor decomposition[J]. **Frontiers** in Bioengineering and Biotechnology, 2022, 10: 911769.     **[[Download]](https://www.frontiersin.org/journals/bioengineering-and-biotechnology/articles/10.3389/fbioe.2022.911769/full)**
    6. 【**SNMDA (**Liu et al., **2024)**】Liu Y, Lin J, Liang P, et al. Potential microRNA-disease association prediction using node2vec and singular value decomposition[J]. IEEE Access, 2024.    **[[Download]](https://ieeexplore.ieee.org/abstract/document/10632126)**  [**[Code**](https://github.com/Ouyang-Dong/SPLHRNMTF)
    7. 【**SPLHRNMTF  (**Ouyang et al., **2024)**】Ouyang D, Miao R, Zeng J, et al. SPLHRNMTF: robust orthogonal non-negative matrix tri-factorization with self-paced learning and dual hypergraph regularization for predicting miRNA-disease associations[J]. BMC genomics, 2024, 25(1): 885.    **[[Download]](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-024-10729-w#Abs1)**  [**[Code**](https://github.com/Ouyang-Dong/SPLHRNMTF)
    8. 【**L2,1 S-NPFM** **(**Xie et al., **2025)**】Xie G, Li W, Gu G, et al. A MiRNA-Disease Association Prediction Method Integrating Graph Matrix Factorization With L $ _ {21} $ similarity Constraint And Network Projection Fusion[J]. IEEE Transactions on Computational Biology and Bioinformatics, 2025.    [**[Download]**](https://ieeexplore.ieee.org/abstract/document/10839520)
- **Machine Learning-based Methods**
    
    ### **Random Forest**
    
    1. 【**RFMDA** (Chen et al., **2018**)】Chen X, Wang C C, Yin J, et al. Novel human miRNA-disease association inference based on random forest[J]. Molecular therapy Nucleic acids, 2018, 13: 568-579.   [**[Download]**](https://www.cell.com/molecular-therapy-family/nucleic-acids/fulltext/S2162-2531(18)30276-2) 
    2. 【**IRFMDA** (Yang et al., 2019)】Yao D, Zhan X, Kwoh C K. An improved random forest-based computational model for predicting novel miRNA-disease associations[J]. BMC bioinformatics, 2019, 20: 1-14.  
    3. 【**Ji's method**（**GraRep-RF）** (Ji et al., 2020)】Ji B Y, You Z H, Cheng L, et al. Predicting miRNA-disease association from heterogeneous information network with GraRep embedding model[J]. Scientific reports, 2020, 10(1): 6658.   [[Download]](https://www.nature.com/articles/s41598-020-63735-9)   [[Code]](https://github.com/jiboya123/working-code.git)  
    4. 【**MGCNRF** (Yang et al., **2023**)】Yang Y, Sun Y, Li F, et al. MGCNRF：Prediction of disease-related miRNAs based on multiple graph convolutional networks and random forest[J]. IEEE Transactions on Neural Networks and Learning Systems, 2023.    [[Download]](https://ieeexplore.ieee.org/abstract/document/10184955)   [[Code]](https://github.com/Changlong2020/ELMDA)  
    
    ### **XGBoost**
    
    1. 【**EGBMMDA  (**Chen et al., **2018)**】Chen X, Huang L, Xie D, et al. EGBMMDA: extreme gradient boosting machine for MiRNA-disease association prediction[J]. Cell death & disease, 2018, 9(1): 3.   [**[Download]**](https://www.nature.com/articles/s41419-017-0003-x)
    2. 【**ELMDA (**Gu et al., **2023)**】Gu C, Li X. Prediction of disease-related miRNAs by voting with multiple classifiers[J]. BMC bioinformatics, 2023, 24(1): 177.     [[Download]](https://link.springer.com/article/10.1186/s12859-023-05308-x)   [[Code]](https://github.com/Changlong2020/ELMDA) 
    
    ### **Regularized Least Square**
    
    1. 【**MKRMDA  (**Chen et al., **2017)**】Chen X, Niu Y W, Wang G H, et al. MKRMDA: multiple kernel learning-based Kronecker regularized least squares for MiRNA–disease association prediction[J]. Journal of Translational Medicine, 2017, 15: 1-14.   [[Download]](https://link.springer.com/article/10.1186/s12967-017-1340-3)   [[Code]](http://www.cuilab.cn/files/images/cuilab/misim.zip)  
    2. 【**KRLSM (**Luo et al., **2017)**】Luo J, Xiao Q, Liang C, et al. Predicting MicroRNA-disease associations using Kronecker regularized least squares based on heterogeneous omics data[J]. Ieee Access, 2017, 5: 2503-2513.    [[Download]](https://ieeexplore.ieee.org/abstract/document/7862218/)   [[Code]](https://github.com/XIAO-HN/KRLSM)  
    3. 【**MKGAT (**Luo et al., 2022**)**】Wang W, Chen H. Predicting miRNA-disease associations based on graph attention networks and dual Laplacian regularized least squares[J]. Briefings in Bioinformatics, 2022, 23(5): bbac292.   [[Download]](https://academic.oup.com/bib/article/23/5/bbac292/6645486?login=false)   [[Code]](https://github.com/shine-lucky/MKGAT-main)  
    4. 【**MLRDFM (**Luo et al., 2022**)**】Ding Y, Lei X, Liao B, et al. MLRDFM: a multi-view Laplacian regularized DeepFM model for predicting miRNA-disease associations[J]. Briefings in bioinformatics, 2022, 23(3): bbac079.     [[Download]](https://academic.oup.com/bib/article/23/3/bbac079/6552270?login=false)   [[Code]](https://github.com/XYDBCS/MLRDFM)  
    
    ### **Others**
    
    1. 【**RLSMDA (**Chen et al., 2014**)**】Chen X, Yan G Y. Semi-supervised learning for potential human microRNA-disease associations inference[J]. Scientific reports, 2014, 4(1): 5501.   [[Download]](https://www.nature.com/articles/srep05501)
    2. 【**DWMDA (**Luo et al., 2025**)**】Ha J. DeepWalk-Based Graph Embeddings for miRNA–Disease Association Prediction Using Deep Neural Network[J]. Biomedicines, 2025, 13(3): 536.   **MDPI**   [[Download]](https://www.mdpi.com/2227-9059/13/3/536) 
- **Deep Learning-based Methods**
    
    ### **Autoencoder**
    
    1. 【**DeepMDA**  (Fu et al., **2017**)**】**Fu L, Peng Q. A deep ensemble model to predict miRNA-disease association, Scientific Reports 2017;7(1):14482. [**[Download]**](https://www.nature.com/articles/s41598-017-15235-6) [**[Code]**](https://github.com/sperfu/DeepMDA)
    2. 【**MDA-CNN**  (Peng et al., **2019**)】 Peng J, Hui W, Li Q et al. A learning-based framework for miRNA-disease association identification using neural networks, Bioinformatics 2019;35(21):4364-4371. [**[Download]**](https://academic.oup.com/bioinformatics/article/35/21/4364/5448859?login=false)  [**[Code]](https://github.com/Issingjessica/MDA-CNN)**  
    3. **【MDA-CF**  (Dai et al., **2021**)**】**Dai Q, Chu Y, Li Z et al. MDA-CF: Predicting MiRNA-Disease associations based on a cascade forest model by fusing multi-source information, Computers in Biology and Medicine 2021;136:104706. [**[Download]**](https://www.sciencedirect.com/science/article/pii/S001048252100500X) [**[Code]**](https://github.com/a1622108/MDA-CF)
    4. 【**AEMDA** (Ji et al., **2021**)】 Ji C, Gao Z, Ma X, et al. AEMDA: inferring miRNA–disease associations based on deep autoencoder[J]. Bioinformatics, 2021, 37(1): 66-72.   [**[Download]**](https://academic.oup.com/bioinformatics/article/37/1/66/5877939?login=false) [**[Code]**](https://github.com/CunmeiJi/AEMDA)
    5. 【**SMALF**  (Liu et al., **2021**)】Liu D, Huang Y, Nie W et al. SMALF: miRNA-disease associations prediction based on stacked autoencoder and XGBoost, BMC Bioinformatics 2021;22(1):219.  [**[Download]**](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04135-2)   [**[Code**](https://github.com/dayunliu/SMALF)
    6. **【DANE-MDA**  (Ji et al., **2021**)**】**Ji B-Y, You Z-H, Wang Y et al. DANE-MDA: Predicting microRNA-disease associations via deep attributed network embedding, iScience 2021;24(6):102455. [**[Download]**](https://www.sciencedirect.com/science/article/pii/S2589004221004235) [**[Code]**](https://github.com/jiboya123/DANE-MDA)
    7. **【SAEMDA**  (Wang et al., **2022**)**】**Wang C C, Li T H, Huang L, et al. Prediction of potential miRNA–disease associations based on stacked autoencoder[J]. Briefings in bioinformatics, 2022, 23(2): bbac021.  [**[Download]**](https://academic.oup.com/bib/article-abstract/23/2/bbac021/6529883?login=false) [**[Code]**](https://github.com/xpnbs/SAEMDA)
    8. **【DFELMDA**  (Liu et al., **2022**)**】**Liu W, Lin H, Huang L et al. Identification of miRNA–disease associations via deep forest ensemble learning based on autoencoder, Briefings in Bioinformatics 2022;23(3). [**[Download]**](https://academic.oup.com/bib/article-abstract/23/3/bbac104/6553934?login=false) [**[Code]**](https://github.com/Zj-Teng/DFELMDA)
    
    ### **Convolutional neural network**
    
    1. **【CNNDMP** (Xuan et al., **2018**)】 Xuan P, Dong Y, Guo Y et al. Dual Convolutional Neural Network Based Method for Predicting Disease-Related miRNAs, International journal of molecular sciences 2018;19(12):3732. [**[Download**](https://www.mdpi.com/1422-0067/19/12/3732)
    2. **【CNNMDA** (Xuan et al., **2019**)】 Xuan P, Sun H, Wang X et al. Inferring the Disease-Associated miRNAs Based on Network Representation Learning and Convolutional Neural Networks, International journal of molecular sciences 2019;20(15):3648. [**[Download]**](https://www.mdpi.com/1422-0067/20/15/3648)
    3. **【DNRLCNN** (Zhong et al., **2022**)】 Zhong J, Zhou W, Kang J et al. DNRLCNN: A CNN Framework for Identifying MiRNA–Disease Associations Using Latent Feature Matrix Extraction with Positive Samples, Interdisciplinary Sciences: Computational Life Sciences 2022;14(2):607-622. [**[Download]**](https://link.springer.com/article/10.1007/s12539-022-00509-z)
    
    ### **Others**
    
    1. 【**EPMDA** (Dong et al., **2019**)】Dong Y, Sun Y, Qin C, et al. EPMDA: edge perturbation based method for miRNA-disease association prediction[J]. IEEE/ACM Transactions on Computational Biology and Bioinformatics, 2019, 17(6): 2170-2175.   [**[Download]](https://ieeexplore.ieee.org/abstract/document/8827911/)  [[Code]](https://github.com/DYDGitHub/EPMDA)**
    2. 【**MvKFN-MDA** (Dong et al., **2021**)】Li J, Liu T, Wang J, et al. MvKFN-MDA: Multi-view Kernel Fusion Network for miRNA-disease association prediction[J]. Artificial Intelligence in Medicine, 2021, 118: 102115.    [**[Download]**](https://www.sciencedirect.com/science/article/abs/pii/S0933365721001081)
    3. 【**PCACFMDA**  (Zhang et al., **2024**)】Zhang C, Li Y, Dong Y, et al. Prediction of miRNA-disease associations based on PCA and cascade forest[J]. BMC bioinformatics, 2024, 25(1): 386.   [[Download]](https://link.springer.com/article/10.1186/s12859-024-05999-w)   [[Code]](https://github.com/zhtdbobo/PCACFMDA) 
- **Graph Network-based Methods**
    
    ### **Graph Convolutional Network (GCN)**
    
    1. 【**NIMCGCN** (Li et al., 2020)】 Li J, Zhang S, Liu T et al. Neural inductive matrix completion with graph convolutional networks for miRNA-disease association prediction, Bioinformatics 2020;36(8):2538-2546. [**[Download]**](https://academic.oup.com/bioinformatics/article/36/8/2538/5697092) [**[Code]**](https://github.com/ljatynu/NIMCGCN/)
    2. 【**MMGCN** (Tang et al., 2021)】 Tang X, Luo J, Shen C et al. Multi-view Multichannel Attention Graph Convolutional Network for miRNA–disease association prediction, Briefings in Bioinformatics 2021;22(6). [**[Download]**](https://academic.oup.com/bib/article-abstract/22/6/bbab174/6271996) [**[Code**](https://github.com/Txinru/MMGCN)
    3. **【MGCNSS (**Li et al., **2024)**】Tian Z, Han C, Xu L, et al. Mgcnss: mirna–disease association prediction with multi-layer graph convolution and distance-based negative sample selection strategy[J]. Briefings in Bioinformatics, 2024, 25(3): bbae168.   [**[Download]**](https://academic.oup.com/bib/article/25/3/bbae168/7645839?login=false) [**[Code]**](https://github.com/15136943622/MGCNSS/tree/master)
    4. 【**MHMDA (**Li et al., **2025)**】Li R, **Ning Q**, aomiao Zhao Y, et al. MHMDA:“Similarity-Association-Similarity” **Metapaths** and **Heterogeneous-Hyper Network** Learning for MiRNA-Disease Association Prediction[J]. IEEE Transactions on Computational Biology and Bioinformatics, 2025.   [**[Download]](https://ieeexplore.ieee.org/abstract/document/10819938)  [[Code]](https://github.com/ningq669/MHMDA/)**
    
    ### **Graph Attention Network (GAT)**
    
    1. 【**MDPBMP** (Yu et al., 2022)】Yu L, Zheng Y, Gao L. MiRNA–disease association prediction based on meta-paths, Briefings in Bioinformatics 2022;23(2).   [**[Download]**](https://academic.oup.com/bib/article-abstract/23/2/bbab571/6501422) [**[Code]**](https://github.com/LiangYu-Xidian/MDPBMP)
    2. 【**MKGAT (**Luo et al., 2022**)**】Wang W, Chen H. Predicting miRNA-disease associations based on graph attention networks and dual Laplacian regularized least squares[J]. Briefings in Bioinformatics, 2022, 23(5): bbac292.   [[Download]](https://academic.oup.com/bib/article/23/5/bbac292/6645486?login=false)   [[Code]](https://github.com/shine-lucky/MKGAT-main)  
    3.  【**HGANMDA** (Li  et al., 2022)**】** Li Z, Zhong T, Huang D et al. Hierarchical graph attention network for miRNA-disease association prediction, Molecular Therapy 2022;30(4):1775-1786. [**[Download]**](https://www.sciencedirect.com/science/article/pii/S1525001622000806) [**[Code]**](https://github.com/ZTangBo/HGANMDA)
    4. **【GRPAMDA**  (Zhong et al., 2022)**】** Zhong T, Li Z, You Z-H et al. Predicting miRNA–disease associations based on graph random propagation network and attention network, Briefings in Bioinformatics 2022;23(2). [**[Download]**](https://academic.oup.com/bib/article-abstract/23/2/bbab589/6515233) [**[Code]**](https://github.com/ZTangBo/GRPAMDA)
    5. 【**MHXGMDA**  (Wen et al., **2024**)】Wen S J, Liu Y B, Yang G, et al. A method for miRNA-disease association prediction using machine learning decoding of multi-layer heterogeneous graph Transformer encoded representations[J]. Scientific Reports, 2024, 14(1): 20490.   [[Download]](https://www.nature.com/articles/s41598-024-68897-4)   [[Code]](https://github.com/yinboliu-git/MHXGMDA)  
    
    ### **Graph Autoencoder (GAE)**
    
    1. **【GAEMDA** (Li et al., 2021)**】** Li Z, Li J, Nie R, et al. A graph auto-encoder model for miRNA-disease associations prediction[J]. Briefings in bioinformatics, 2021, 22(4): bbaa240.[**[Download]**](https://academic.oup.com/bib/article/22/4/bbaa240/5929824?login=false#273162371) [**[Code**](https://github.com/chimianbuhetang/GAEMDA)
    2.  【**VGAMF** (Shi et al., 2021)**】** Ding Y, Lei X, Liao B, et al. Predicting miRNA-disease associations based on multi-view variational graph auto-encoder with matrix factorization[J]. IEEE journal of biomedical and health informatics, 2021, 26(1): 446-457. [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9451570) [**[Code]**](https://github.com/XYDBCS/VGAMF)
    3. **【AGAEMD** (Zhang et al., 2022)**】** Zhang H, Fang J, Sun Y, et al. Predicting miRNA-disease associations via node-level attention graph auto-encoder[J]. IEEE/ACM Transactions on Computational Biology and Bioinformatics, 2022, 20(2): 1308-1318.  [**[Download]**](https://ieeexplore.ieee.org/abstract/document/9767602) [**[Code]**](https://github.com/Zhhuizhe/AGAEMD)
    4. **【ReHoGCNES-MDA** (Zhang et al., 2024)**】** Zhang Y, Chu Y, Lin S, et al. ReHoGCNES-MDA: prediction of miRNA-disease associations using homogenous graph convolutional networks based on regular graph with random edge sampler[J]. Briefings in Bioinformatics, 2024, 25(2): bbae103. [**[Download]**](https://academic.oup.com/bib/article/25/2/bbae103/7631472?login=false#444502587) [**[Code]**](https://github.com/yufangz-sjtu/ReHoGCNES-MDA)
    
    ### **Graph Neural Network (GNN)**
    
    1. 【**SGLMDA**  (Ji et al., 2024)】Ji C, Yu N, Wang Y, et al. SGLMDA: A subgraph learning-based method for miRNA-disease association prediction[J]. IEEE/ACM Transactions on Computational Biology and Bioinformatics, 2024.   [**[Download]](https://ieeexplore.ieee.org/abstract/document/10461041)  [[Code]](https://github.com/CunmeiJi/SGLMDA)**
    2. 【**HHOMR  (**Li et al., **2024)**】Li Z, Wan L, Wang L, et al. HHOMR: a hybrid high-order moment residual model for miRNA-disease association prediction[J]. Briefings in Bioinformatics, 2024, 25(5): bbae412.    [**[Download]](https://academic.oup.com/bib/article/25/5/bbae412/7739100?login=false)**   [**[Code]**](https://github.com/W-LP/HHOMR)
    3. 【**SFPred** (Xuan et al., 2025)】Xuan P, Qi X, Chen S, et al. Subgraph Topology and Dynamic Graph Topology Enhanced Graph Learning and Pairwise Feature Context Relationship Integration for Predicting Disease-Related miRNAs[J]. Journal of Chemical Information and Modeling, 2025. [**[Download]**](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.4c01757) [**[Code]**](https://github.com/pingxuan-hlju/SFPred)
    
    ### **Hypergraph Neural Network (HGNN)**
    
    1. 【**AMHMDA**  (Ning et al., 2023)】**Ning Q**, Zhao Y, Gao J, et al. AMHMDA: attention aware multi-view similarity networks and hypergraph learning for miRNA–disease associations identification[J]. Briefings in Bioinformatics, 2023, 24(2): bbad094.   [**[Download]**](https://academic.oup.com/bib/article/24/2/bbad094/7076121?login=false#398981478)   [**[Code]**](https://github.com/ningq669/AMHMDA)
    2. 【**MHCLMDA** (Peng et al., **2024**)】Peng W, He Z, Dai W, et al. MHCLMDA: multihypergraph contrastive learning for miRNA–disease association prediction[J]. Briefings in Bioinformatics, 2024, 25(1): bbad524. [**[Download]**](https://academic.oup.com/bib/article/25/1/bbad524/7571388?login=false) [**[Code]**](https://github.com/weiba/MNGCL)
    3. 【**HGCLAMIR** (Ouyang et al., **2024**)】Ouyang D, Liang Y, Wang J, et al. Hgclamir: Hypergraph contrastive learning with attention mechanism and integrated multi-view representation for predicting mirna-disease associations[J]. PLOS Computational Biology, 2024, 20(4): e1011927.    [**[Download]**](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1011927)
    4. 【**HHMDA** (Dai et al., 2025)】Dai W, Pang S, He Z, et al. Prediction of miRNA-disease association based on heterogeneous hypergraph convolution and heterogeneous graph multi-scale convolution[J]. Health Information Science and Systems, 2025, 13(1): 1-13. [**[Download]**](https://link.springer.com/article/10.1007/s13755-024-00319-1) [**[Code**](https://github.com/weiba/HHMDA)
    5. 【**HeMDAP** (Ma et al., **2025**)】Ma Y, Wang F, Feng Q, et al. HeMDAP: Heterogeneous Graph Self-Supervised Learning for MiRNA-Disease Association Prediction[J]. **IEEE Transactions on Computational Biology and Bioinformatics**, 2025.    [**[Download]](https://ieeexplore.ieee.org/abstract/document/10857657)  [[Code]](https://github.com/IDATA-health/HeMDAP)**
    6. 【**CLHGNNMDA** (Zhu et al., **2025**)】Zhu R, Wang Y, Dai L Y. CLHGNNMDA: Hypergraph Neural Network Model Enhanced by Contrastive Learning for miRNA–Disease Association Prediction[J]. Journal of Computational Biology, 2025, 32(1): 47-63.   [**[Download]**](https://www.liebertpub.com/doi/abs/10.1089/cmb.2024.0720)   [**[Code]**](https://github.com/zhurong1942/CLHGNNMDA_zr1)



## Welcome to contribute
If you would like to help contribute this list, please feel free to contact me by email:

* Email: siya.xie@mpu.edu.mo
