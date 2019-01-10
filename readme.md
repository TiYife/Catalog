# Lecture-1 数据挖掘简介
## 什么是数据挖掘： p7
## 数据挖掘和机器学习： p7
## 特征的评价方式：p8
* 新颖、使用、简洁、确定
## 数据挖掘的动力：p11
* 科学角度
* 商业角度
* 日常生活
## 处理什么样的数据-18
## 有什么功能-19
* 预测功能       
* 描述功能
* 特征发掘、特征关联性、相关性、因果性分析
* 分类和预测
* 聚类分析
* 离群点预测
* 趋势和演变分析
## 分类-22
## 聚类-29
## 序列特征发掘-39
## 回归-41
## 离群分析-42
## KDD process（knowledge discovery in database）-43
* KDD的步骤-44 



# Lecutre-2 数据预处理
## 数据-3
### 数据类型-5
    nominal ,ordinal ,interval ,ratio 
### 数据属性-8
    几何平均数、调和平均数
### 离散型和连续性-10
### 数据集-11
* 类型: record, ordered , graph 
* 特征: dimensionality, sparsity, skewness(偏斜)
## 数据预处理-23
### 为什么要数据预处理-23
    incomplete,noisy,inconsist,duplicat
### 数据质量评价指标-26
    accuracy, completeness, consistency, timeliness, believability, value added, interpretability, accessibility
### 数据预处理的主要工作-27
    数据清洗、数据整合、数据转换、数据化简、数据离散化
    clearning integration transformation  reduction discretization
## 数据摘要-29
### 数据属性
    中位数、最大值、最小、分位数、离群点、方差
### 描述中心属性-30
#### 均值、中位数、峰值
    mean、median、mode
$2*mean = 3*median-mode$

    中值一定在均值和峰值之间，根据倾斜方向可以确定左右哪个是峰值哪个是均值
#### 马尔科夫不等式-32
* $$P(X \ge a)\le \frac{E(X)}{a}$$
* $$a \times P(X \ge a) = E(Y) \le E(X)$$
* $$a = k \times E(X), P(X \ge a) \le \frac{E(X)}{K \times E(X)}= \frac 1k$$
### 描述分散属性-34

#### 方差-34、标准差-35、z-score-36
$$Var(X)=E[(X-\mu)^2]=E(X^2)-E^2(X)$$
#### 切比雪夫不等式-37
* $$P(|X-\mu|\ge a)\le \frac{\sigma^2}{a^2}$$
* $$ a= k\sigma, \ then \  P(|X - \mu|\ge k\sigma )\le \frac{\sigma^2}{k^2\sigma^2}=\frac1{k^2}$$
#### 霍夫丁不等式-40
#### 正态分布 -41
    68-95-99.7
### 框图分析-45（boxplot）
### 直方图分析-47 （histogram）
### 分位数 - 52
### Q-Q Plot-53
### 散点图-54（Scatter）
### Loess Curve -55


# Lecture-3 数据预处理
## 数据清洗
### 重要性-3
### 清洗工作-3
* 填充、辨别离群点、平滑噪声、校准不一致数据、去冗余
*  缺失数据-4
* 噪声数据-6
    * 装箱-8
    * 聚类-10
    * 回归-11
    * 人工判断
## 数据整合和转换
### 数据整合-13
* 处理整合过程中的冗余-14
    * 关联分析-15
        * 协方差-15
        * 相关系数-17
        * $\chi^2$ -20
### 数据转换-24
* normalization -24
    * min-max normalization
    * z-score normalization
    * normalization by decimal scaling
## 数据化简
### 化简策略 -26
* 数量上化简
    * 参数化方法
        * 回归分析 -28
    * 非参数化方法
        * 直方图 -29
        * 聚类 -30
        * 采样 -31
* 降低维度-34
    * 特征选择
        * 启发式特征选择 -35
    * 空间转换
### 主成分分析-37
## 离散化和概念层次生成
### 离散化-55
### 概念层次-56
### 离散化/概念层次
* 数字数据-57
    * 熵（Entropy）-58
    * $\chi^2$-59
    * 基于自然间隔的分段-60
* 类型数据-62
## one-hot
### 对类型数据的处理-65


# Lecture-4 频繁项集挖掘、关联和相关性分析
## 频繁项集
### 概念-3
### 频繁特征和关联规则-6
* 相对支持度、绝度支持度、支持度、置信度 -6
* 闭合项集、最大特征 -7
## 频繁项挖掘方法
* 演绎（Apriori）-11
* Pattern growth-22
* apriori VS FP growth -33
* 项集生成器 - 36
* Vertical data format approach
## 从关联挖掘到相关性分析
## 基于约束的关联挖掘
## 序列特征挖掘


# Lecture-5 频繁项集挖掘、关联和相关性分析
## 频繁项挖掘方法
* A-close : breath-first search based
* CLOSET/CLOSET+ : FP-tree and depth-first search based
* MAFIA : vertical bitmap representation
* CHARM : vertical data representation and diffset technique
### 对比点-9
* search order
    * breadth-first
    * depth-first
* data representation
    * horizontal 
    * vertical
* data compression
    * FP-tree
    * diffset
* search space pruning
    * item merging
    * sub-itemset pruning
### CHARM ---- fast vertical closed itemset mining using diffset  -12
### CLOSET+ ---- searching for the besh strategies for mining frequent closed itemsets
### closed vs. frequent/ CLOSET+ vs. CHARM 
## 从关联挖掘到相关性分析
### 相关性评价指标 
* lift -44
* $\chi^2$ -45
## 基于约束的关联挖掘
### 数据挖掘中的约束-49
* 数据约束
* 维度约束
* 特征约束
* 关注点约束
    * 反单调约束-50
    * 单调约束-52
    * 简要约束-54
    * 可转换约束-60
    * 复杂约束-65


# Lecture-6 序列特征挖掘
## 频繁序列和闭合序列
* 定义 -4
* 为什么挖掘频繁序列 -5
* 为什么挖掘闭合序列 -6
## 序列特征挖掘方法
    GSP, SPADE, PrefixSpan，SPAM
* GSP -9
* SPADE -14
* GSP和SPADE 的缺陷 -16
* PrefixSpan -17
## 闭合序列挖掘方法
    CloSpan, BIDE
* CloSpan -25
* BIDE -30
    * an efficient closed sequential pattern mining algorthm 
    * BI-Directional Extension closrue checking -35
    * BackScan search space pruning -40
    * ScanSkip optimization technique -41 


# Lecture-7 图数据挖掘
## Motivation -4
## Definition -7
## Challenges -10
* pattern growing -12
* Candidate subgraph multiplicity -14
* Graph isomorphism -18
    * use canonical labeling to handle isomorphism -22
##  Typical algorithms
### Apriori-like algorthms-24
 * 举例：AGM, FSG,FFSM,... -24
 * 过程 -25
### Pattern-growth algorithms -28
### closed graph -32
## Typical applications- 34
* graph classification -36
* graph clustering -46 
* coherent subgraph mining -54
* graph search -60
* graph modeling for recommender system -67
* graph modeling for entity linking -74
* graph pattern discovery 
* others


# Lecture-8 分类和预测
## 分类
* 分类定义 -3
    * 构建模型
    * 用模型预测
* 分类 vs 预测 -8
* 有监督 vs 无监督 -9
## 分类相关的内容
* 数据预处理 -11
    * 数据清洗
    * 相关分析
    * 数据转换
* 评估指标 -12
    * 准确性
    * 速度
    * 鲁棒性
    * 可拓展性
    * 可解释性
## 预测 
* 预测定义-14
* 线性回归 -15
    * 梯度下降 -17 
    * 标准方程 - 20
* 非线性回归 -22
* 逻辑回归 -23
* rating prediction：latent factor models -34


# Lecture-9 分类和预测
## 决策树
* 基本算法 -6
* 中值条件 -6
* 属相选择标准 -7
    *  熵 -10
    * 信息增益 -12
        * 连续数据的信息增益 -14
        * 高分支属性 -15
    * 收益率 -18
    * 基尼指数 -20
    * 信息增益 vs 收益率 vs 基尼指数 -22
    * CHAID -23
* 过拟合和树裁剪 -25
* 拓展决策树 -26
* 大数据库中的分类 -27
## 基于规则的分类
* 基本概念 -34
    * coverage
    * accuracy
    * conflict resolution strategy
* 从决策树中抽取规则 -35
* sequential covering algorithm（序列覆盖？） -37
* Fiol-gain -38
* Foil缺陷 -40
* CPAR -40 
* Instance-Centric -45
* HARMONY -48 
## 关联分类 （association classification）
* 定义 -61
* 典型算法 -62
    * CBA -63
    * CMAR -66
    

# Lecture-10 贝叶斯+最近邻
## 贝叶斯 
* 基本概念 -4
* 原理 -5
* 朴素贝叶斯 -6
* 具体算法 （明天细看）
## k近邻
* k紧邻算法 - 19
* KNN 推荐系统 -21
* cololaborative filtering -22


# Lecture-11 人工神经网络+支持向量机
## 人工神经网络
* 基本概念 -3
* 基本结构 -7
* 常见功能 -8
* 网络结构 -9
* McCullock and Pitts Perceptron model -10
* 多层神经网络 -14
    * 如何运作 -15
    * 反向传播
    * a neuron
* multi-layer feed-forward neural network -18
* 网络拓扑 -22
* 反向传播和可解释性 -23
* 神经网络 vs 分类器
## SVM
* 概念 -26
* 基本原理 -28
* 线性关系 -35
* 非线性关系 -39
* 核函数 -45
* SVM VS 人工神经网络 -47


# Lecture-12 集成学习
## 集成方法 -3
* bagging -5
* boosting -7
    * adaboost -10
* random forest -14
    * rCART -15
    * Byproducts -16
## 准确性和错误度评价 -21
* 准确性评价 -21
    * ROC Curves -22
* 错误性评价 -23
* 准确性评价 -24
    * holdout
    * cross-validation
    * bootstrap


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
