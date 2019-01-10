
# Lecture-13 聚类分析
## 聚类
* 定义 -3
* 评价指标 -5
## 聚类中的数据
* data struct -9
    * data matrix 
    * dissimilarity matrix
* 数据类型 -10
    * interval-scaled variables -11
    * binary variable -14
    * nominal、ordinal、radio variables -16
    * variables of mixed types -19
 ## 主要聚类方法的分类
 * 主要聚类方法 -22
    * partitioning
    * hierarchical 
    * density-based
    * model-based
    * user-guilded/constraint-based
* 典型的距离计算方法 -24
    * single link
    * complete link
    * average
    * centroid 质心
    * medoid
* 质心，半径，直径计算方法 -25
## partitioning
* 基本概念 -27
* K-means -28
* K-medoids -32
    * PAM -33
    * CLARA -37


# Lecture-14 层级聚类+密度聚类+模型聚类
## 层级聚类
* 简介 -3
* AGNES（Agglomerative Nest） -4
* Dendrogram -5
* DIANA（Divisive Analysis） -6
* 层级聚类方法 - 7
    * BIRCH -8
    * ROCK -12
    * CHAMELEON -15

## 密度聚类
* 简介 -19
* 概念 -20
    * density-reachable
    * density-connected
* DBSCAN -22
* CHAMELEON -25

## 模型聚类 
* 简介 -27
* statistical approach
    * EM（expectation maximization）-28
        * MLE -29
* Neural network approach
    * SOM（Self-Organizing Feature Map）-36


# Lecture-15 高维聚类+例外发现
## 高维聚类 
* 简介 -3
* 高维问题 -4
* CLIQUE -6
* Pattern Discovery-Based approach -10
* Clustering by Pattern Similarity -15
    * p-cluster -16

## 例外发现
* 简介 -19
* statistical approaches -20
    * anomaly detection -21
    * density estimation -22
    * anomaly detection vs supervised learning -24
    * Multivariate gaussian distribution -25
    * anomaly detection with multivariate gaussian -26
    * relationship to original model -27
* distance-based approach -28
* density-based local outlier detection -29
* cluster-based approach -30
