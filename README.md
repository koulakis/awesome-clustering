# Awesome Clustering [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

*Last updated 04.03.2025.*

**WARNING: This list is still new and under construction! It still contains incomplete and potentially incorrect information. So use with caution.**

## Contents
<!-- TOC -->
* [Awesome Clustering ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](#awesome-clustering-)
  * [Contents](#contents)
  * [Surveys](#surveys)
  * [Theory](#theory)
  * [Methods](#methods)
  * [Estimating the number of clusters](#estimating-the-number-of-clusters)
  * [Frameworks and code](#frameworks-and-code)
  * [Datasets](#datasets)
<!-- TOC -->

## Surveys

| Year | Authors                                                 | Title                                                                                  | Venue                                               | Publication Link                                                                                                                               |
|------|---------------------------------------------------------|----------------------------------------------------------------------------------------|-----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| 1999 | Jain, Anil K., M. Narasimha Murty, and Patrick J. Flynn | Data clustering: a review                                                              | ACM computing surveys (CSUR)                        | [Link](https://dl.acm.org/doi/pdf/10.1145/331499.331504)                                                                                       |
| 2005 | Xu, Rui, and Donald Wunsch                              | Survey of clustering algorithms                                                        | IEEE Transactions on neural networks                | [Link](https://www.researchgate.net/publication/3303538_Survey_of_Clustering_Algorithms)                                                       |
| 2015 | Xu, Dongkuan, and Yingjie Tian                          | A comprehensive survey of clustering algorithms                                        | Annals of data science                              | [Link](https://link.springer.com/article/10.1007/S40745-015-0040-1)                                                                            |
| 2022 | Ezugwu, Absalom E., et al.                              | A Comprehensive Survey on Deep Clustering: Taxonomy, Challenges, and Future Directions | Engineering Applications of Artificial Intelligence | [Link](https://www.researchgate.net/publication/361323843_A_Comprehensive_Survey_on_Deep_Clustering_Taxonomy_Challenges_and_Future_Directions) |


## Theory
| Year | Authors                            | Title                                                                                                  | Venue                                             | Publication Link                                                                                              |
|------|------------------------------------|--------------------------------------------------------------------------------------------------------|---------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| 2017 | Moseley, Benjamin and Wang, Joshua | Approximation Bounds for Hierarchical Clustering: Average Linkage, Bisecting K-means, and Local Search | Advances in Neural Information Processing Systems | [Link](https://proceedings.neurips.cc/paper_files/paper/2017/file/d8d31bd778da8bdd536187c36e48892b-Paper.pdf) |


## Methods
| Year                    | Authors                                                | Title                                                                            | Venue                                                                             | Method Abbreviation | Publication Link                                                                                                                                                           | Code Link                                                                                                     |
|-------------------------|--------------------------------------------------------|----------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| 1958                    | RR, SOKAL. et al.                                      | A statistical method for evaluating systematic relationships                     | University of Kansas Science Bulletin                                             | HAC                 | [Link](https://ia802205.us.archive.org/13/items/cbarchive_33927_astatisticalmethodforevaluatin1902/astatisticalmethodforevaluatin1902.pdf)                                 | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)        |
| 1963                    | Ward Jr, Joe H.                                        | Hierarchical grouping to optimize an objective function                          | Journal of the American statistical association                                   | HAC                 | [Link](https://ia802205.us.archive.org/13/items/cbarchive_33927_astatisticalmethodforevaluatin1902/astatisticalmethodforevaluatin1902.pdf)                                 | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)        |
| 1967                    | Lance, Godfrey N., and William Thomas Williams         | A general theory of classificatory sorting strategies: 1. Hierarchical systems   | The computer journal                                                              | HAC                 | [Link](https://ia802205.us.archive.org/13/items/cbarchive_33927_astatisticalmethodforevaluatin1902/astatisticalmethodforevaluatin1902.pdf)                                 | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)        |
| 1970                    | Cheeger, Jeff.                                         | A lower bound for the smallest eigenvalue of the Laplacian                       | Problems in analysis                                                              | Spectral Clustering | [Link](https://www.degruyter.com/document/doi/10.1515/9781400869312-013/pdf?licenseType=restricted)                                                                        | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.SpectralClustering.html)             |
| 1982 (proposed in 1957) | Lloyd, Stuart                                          | Least squares quantization in PCM                                                | IEEE transactions on information theory                                           | k-means             | [Link](https://hal.science/hal-04614938/document)                                                                                                                          | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)                         |
| 1996                    | Ester, Martin, et al.                                  | Density-based spatial clustering of applications with noise                      | Int. Conf. knowledge discovery and data mining                                    | DBSCAN              | [Link](https://www.dbs.ifi.lmu.de/Publikationen/Papers/KDD-96.final.frame.pdf)                                                                                             | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html)                         |
| 2001                    | Ng, Andrew, Michael Jordan, and Yair Weiss             | On spectral clustering: Analysis and an algorithm                                | Advances in neural information processing systems                                 | Spectral Clustering | [Link](https://ai.stanford.edu/~ang/papers/nips01-spectral.pdf)                                                                                                            | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.SpectralClustering.html)             |
| 2006                    | Arthur, David, and Sergei Vassilvitskii                | k-means++: The advantages of careful seeding                                     | arXiv preprint                                                                    | k-means++           | [Link](https://theory.stanford.edu/~sergei/papers/kMeansPP-soda.pdf)                                                                                                       | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) (with init="k-means++") |
| 2013                    | Campello, Ricardo JGB, Davoud Moulavi, and Jörg Sander | Density-based clustering based on hierarchical density estimates                 | Pacific-Asia conference on knowledge discovery and data mining                    | HDBSCAN             | [Link](https://www.researchgate.net/publication/315508524_hdbscan_Hierarchical_density_based_clustering)                                                                   | [Code](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.HDBSCAN.html)                        |
| 2013                    | Elhamifar, Ehsan, and René Vidal                       | Sparse subspace clustering: Algorithm, theory, and applications                  | IEEE transactions on pattern analysis and machine intelligence                    | SSC                 | [Link](https://arxiv.org/abs/1203.1005)                                                                                                                                    | [Code](https://github.com/abhinav4192/sparse-subspace-clustering-python)                                      |
| 2019                    | Sarfraz, Saquib, Vivek Sharma, and Rainer Stiefelhagen | Efficient parameter-free clustering using first neighbor relations               | Proceedings of the IEEE/CVF conference on computer vision and pattern recognition | FINCH               | [Link](https://openaccess.thecvf.com/content_CVPR_2019/papers/Sarfraz_Efficient_Parameter-Free_Clustering_Using_First_Neighbor_Relations_CVPR_2019_paper.pdf)              | [Code](https://github.com/ssarfraz/FINCH-Clustering)                                                          |
| 2021                    | Sarfraz, Saquib, et al.                                | Temporally-weighted hierarchical clustering for unsupervised action segmentation | Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition | TW-FINCH            | [Link](https://openaccess.thecvf.com/content/CVPR2021/papers/Sarfraz_Temporally-Weighted_Hierarchical_Clustering_for_Unsupervised_Action_Segmentation_CVPR_2021_paper.pdf) | [Code](https://github.com/ssarfraz/FINCH-Clustering/tree/master/TW-FINCH)                                     |
| 2022                    | Ronen, Meitar, Shahaf E. Finder, and Oren Freifeld     | Deepdpm: Deep clustering with an unknown number of clusters                      | Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition | DeepDPM             | [Link](https://openaccess.thecvf.com/content/CVPR2022/papers/Ronen_DeepDPM_Deep_Clustering_With_an_Unknown_Number_of_Clusters_CVPR_2022_paper.pdf)                         | [Code](https://github.com/BGU-CS-VIL/DeepDPM)                                                                 |


## Estimating the number of clusters
| Year | Authors                                                 | Title                                                                 | Venue                                    | Publication Link                                  | Code Link                                             |
|------|---------------------------------------------------------|-----------------------------------------------------------------------|------------------------------------------|---------------------------------------------------|-------------------------------------------------------|
| 2001 | Tibshirani, Robert, Guenther Walther, and Trevor Hastie | Estimating the number of clusters in a data set via the gap statistic | Journal of the royal statistical society | [Link](https://tibshirani.su.domains/ftp/gap.pdf) | [Code](https://github.com/milesgranger/gap_statistic) |


## Frameworks and code
| Name         | Language | Methods                                                | Documentation                                                    | Code                                                 |
|--------------|----------|--------------------------------------------------------|------------------------------------------------------------------|------------------------------------------------------|
| scikit-learn | python   | k-means, k-means++, dbscan, hdbscan, spectral and more | [Docs](https://scikit-learn.org/stable/api/sklearn.cluster.html) | [Code](https://github.com/scikit-learn/scikit-learn) |

## Datasets
