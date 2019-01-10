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
