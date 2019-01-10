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
