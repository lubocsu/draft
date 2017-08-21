基于内容的推荐（Content-based Recommendations）
--

1. Item Representation：为每个item抽取出一些特征（也就是item的content了）来表示此item；
2. Profile Learning：利用一个用户过去喜欢（及不喜欢）的item的特征数据，来学习出此用户的喜好特征（profile）；
3. Recommendation Generation：通过比较上一步得到的用户profile与候选item的特征，为此用户推荐一组相关性最大的item。

步骤一：文章的标签
步骤二：用户行为 
步骤三：分析用户可能性

### 特征提取

分词库：[jieba](https://github.com/fxsjy/jieba) 功能：

 - 基于前缀词典实现高效的词图扫描，生成句子中汉字所有可能成词情况所构成的有向无环图 (DAG)
 - 采用了动态规划查找最大概率路径, 找出基于词频的最大切分组合
 - 对于未登录词，采用了基于汉字成词能力的 HMM 模型，使用了 Viterbi 算法

分词功能

 - 基于 TF-IDF 算法的关键词抽取
 - 基于 TextRank 算法的关键词抽取

**TextRank**

> TextRank算法可以用来从文本中提取关键词和摘要（重要的句子）

 - 关键词提取
 - 关键短语提取
 - 摘要生成

中文库：[https://github.com/letiantian/TextRank4ZH](https://github.com/letiantian/TextRank4ZH)

**LDA**

> 隐含狄利克雷分布简称LDA(Latent Dirichlet allocation)，是一种主题模型，它可以将文档集中每篇文档的主题按照概率分布的形式给出。

### 用户喜好

**最近邻方法（k-Nearest Neighbor，简称kNN）**


**Rocchio算法**

**决策树算法（Decision Tree，简称DT）**

**线性分类算法（Linear Classifer，简称LC）**

**朴素贝叶斯算法（Naive Bayes，简称NB）**

### 生成推荐



协同过滤
---



参考内容：

 - 《驾驭文本》
 - 《推荐系统》
 - 《机器学习实战》
 
文章：[http://www.cnblogs.com/breezedeus/archive/2012/04/10/2440488.html](http://www.cnblogs.com/breezedeus/archive/2012/04/10/2440488.html)
