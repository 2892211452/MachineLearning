# 机器学习

深度学习也是一种机器学习，所以要学习好基础的机器学习，了解基本的概念。

### k邻近算法
属于监督学习
首先先转化为标准向量几何空间中去，然后再计算，看离我们需要预测的点的距离谁最近，统计最近的k个点，跟具这几个点的类别，判断出该点的类别。

### k-means聚类

属于无监督学习

Kmeans算法正是基于这一思想而生，让数据通过某种算法聚集，不再进行划分的方法称为**聚类算法**。

在聚类问题当中，一系列样本被模型根据数据的属性聚合在了一起，成为了同一个类别。这里的类别就称为这些样本的类簇(cluster)。每一个簇的中心点称为簇中心。所以，KMeans算法，顾名思义，就是将样本根据用户设置的K值，**一共聚类成K个类簇**。

### svm向量机




### 决策树
决策树，可以应用在分类，可以搭建图形化的决策树，熵。
### 线性回归算法
线性回归就是构造一条线，能够最程度的拟合数据
机器学习中常见办法：
- 首先计算出构造函数loss（W，B），我们要做的就是尽可能的使得loss要小。那么可以直接求导，找到极值点，然后稍微比较一下既可以得出答案
- 另外一种就是类似我们的深度学习中的随机梯度下降
### 逻辑回归算法 Logistic Regression







### 随机森林算法 Random Forest
在决策树的基础上，用决策树构建一片森林，
主要的思路就是，从样本的行（样本的数量），和列（单个样本的特征数）。分别随机选取。然后搭建随机森里。可以较好解决小批量分类等问题
### 朴素贝叶斯算法 Naive Bayes



在概率论和统计学中，Bayes’ theorem（贝叶斯法则）根据事件的先验知识描述事件的概率。贝叶斯法则表达式如下所示

![img](https://img-blog.csdn.net/20180704164540248?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3p3cWpveQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)

朴素贝叶斯分类的正式定义如下：

1、设![img](http://latex.codecogs.com/gif.latex?x=%5C%7Ba_1,a_2,...,a_m%5C%7D)为一个待分类项，而每个a为x的一个特征属性。

2、有类别集合![img](http://latex.codecogs.com/gif.latex?C=%5C%7By_1,y_2,...,y_n%5C%7D)。

3、计算![img](http://latex.codecogs.com/gif.latex?P(y_1%7Cx),P(y_2%7Cx),...,P(y_n%7Cx))。

4、如果![img](http://latex.codecogs.com/gif.latex?P(y_k%7Cx)=max%5C%7BP(y_1%7Cx),P(y_2%7Cx),...,P(y_n%7Cx)%5C%7D)，则![img](http://latex.codecogs.com/gif.latex?x%20%5Cin%20y_k)。

**朴素贝叶斯算法对条件概率分布作出了独立性的假设**，通俗地讲就是说假设各个维度的特征*x*1,*x*2,...,*x**n*互相独立，在这个假设的前提上，可以简化计算规模，减小运算量。





### 降维算法 Dimensional Reduction

(PCA)是最常用的线性降维方法，它的目标是通过某种线性投影，将高维的数据映射到低维的空间中表示，并期望在所投影的维度上数据的方差最大，以此使用较少的数据维度，同时保留住较多的原数据点的特性。
[PCA原理讲解，很详细](https://blog.csdn.net/lijihw/article/details/46622667?depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-6&utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromBaidu-6)
回顾了一下线代知识和数理统计。 统计学厉害，数学厉害。

### 梯度增强算法 Gradient Boosting
**GTB算法**
决策树的基础上
梯度提升（gradient boosting）算法最初是FreidMan在2000年提出来的，其核心就在于，每棵树是从先前所有树的残差中来学习。利用的是当前模型中损失函数的负梯度值
