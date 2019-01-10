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