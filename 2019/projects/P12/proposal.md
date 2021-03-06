---
layout: page
mathjax: true
permalink: /2019/projects/p12/proposal/
---

> 注意: 上方的内容不要删除

## 项目题目 


### 成员
徐元超(3220180887), 徐金良(3220180885), 杨洋(3220180892)

### 问题描述

#### 1、问题背景分析
现如今，随着互联网和科学技术的高速发展，我们处在信息过载的时代，每个人在日常生活中都会面对海量的信息，
如果不对信息进行筛选在海量的信息中选取自己所感兴趣的信息是一件很难的事情。
如何对这些信息按照人们的喜欢进行个性化筛选就是推荐算法所要做的。我们将选取几种比较经典的推荐算法进行比较，
包括UserCF, ItemCF, LFM, PersonalRank等，数据集采取MovieLens，完成对指定用户电影推荐的任务。
#### 2、问题描述

2.1 数据准备  
MovieLens 1MB数据集，其中包括了用户对电影的评分、标签，以及对应的时间等信息  
2.2 模型建立  
采用基于用户和物品的协同过滤算法和LFM  
User based CF：找出与指定用户最相似的n个用户，指定用户对物品j的兴趣就是这n个用户对物品j的兴趣的加权和。  
Item based CF：找出与物品j最相似的n个物品，指定用户对物品j的兴趣就是用户对这n个物品的兴趣的加权和。  
LFM模型：将评分矩阵分解为两个低维矩阵的乘积，再利用梯度下降法对这两个低维矩阵进行优化，使得模型的RMSE的值达到局部最小值
，便可以利用两个低维矩阵计算指定用户对物品j的兴趣度或评分。 

2.3 预期的结果  
通过用户已有的行为对其进行符合其口味的电影推荐  
### 项目评估
采用精确率，召回率，覆盖率，流行度等指标对不同算法进行评估比较  
### 项目分工
杨洋 UserCF、ItemCF算法，撰写报告  
徐元超 算法调研、数据预处理、撰写报告  
徐金良 LFM算法、撰写报告  
