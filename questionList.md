# 面试题整理

1. 特征点的匹配机制有哪些？
2. 深度学习中评价指标的解释，mAP、PR 曲线、AUC。
3. Tensorflow 的动态图和静态图有什么区别?

## 深度学习

### 模型评估方法

- [Accuracy 作为指标有哪些局限性？](https://github.com/buki26/InterviewQuestions/blob/master/answers/Accuracy%20%E4%BD%9C%E4%B8%BA%E8%AF%84%E4%BB%B7%E6%8C%87%E6%A0%87%E7%9A%84%E5%B1%80%E9%99%90%E6%80%A7.md)
- [ROC 曲线和 PR 曲线各是什么？](https://github.com/buki26/InterviewQuestions/blob/master/answers/ROC%E5%92%8CPR%E6%9B%B2%E7%BA%BF.md)
- 编程实现 AUC 的计算，并指出复杂度？
- AUC 指标有什么特点？放缩结果对 AUC 是否有影响？
- [余弦距离与欧式距离有什么特点？](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E6%AC%A7%E5%BC%8F%E8%B7%9D%E7%A6%BB%E4%B8%8E%E4%BD%99%E5%BC%A6%E8%B7%9D%E7%A6%BB.md)

### 基本方法

- 如何划分训练集？如何选取验证集？
- [什么是偏差和方差？](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E5%81%8F%E5%B7%AE%E5%92%8C%E6%96%B9%E5%B7%AE.md)
- 什么是过拟合？深度学习解决过拟合的方法有哪
- 解决欠拟合的方法有哪些？
- 深度模型参数调整的一般方法论？

### 优化方法

- 简述了解的优化器，发展综述？
- [常用的损失函数有哪些？分别适用于什么场景？](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E5%B8%B8%E8%A7%81%E6%8D%9F%E5%A4%B1%E5%87%BD%E6%95%B0%E5%8F%8A%E5%BA%94%E7%94%A8%E5%9C%BA%E6%99%AF.md)
- [梯度下降与拟牛顿法的异同？](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E6%A2%AF%E5%BA%A6%E4%B8%8B%E9%99%8D%E4%B8%8E%E6%8B%9F%E7%89%9B%E9%A1%BF%E6%B3%95%E7%9A%84%E5%BC%82%E5%90%8C.md)
- L1 和 L2 正则分别有什么特点？为何 L1 稀疏？

### 深度学习基础

- 以一层隐层的神经网络，relu 激活，MSE 作为损失函数推导反向传播
- NN 的权重参数能否初始化为 0？
- [什么是梯度消失和梯度爆炸？](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E6%A2%AF%E5%BA%A6%E6%B6%88%E5%A4%B1%E5%92%8C%E6%A2%AF%E5%BA%A6%E7%88%86%E7%82%B8.md)
- 常用的激活函数，导数？
- [relu 的有优点？又有什么局限性？他们的系列改进方法是啥？](https://github.com/buki26/InterviewQuestions/blob/master/answers/relu%E6%BF%80%E6%B4%BB%E5%87%BD%E6%95%B0%E7%9A%84%E4%BC%98%E7%BC%BA%E7%82%B9%E5%8F%8A%E6%94%B9%E8%BF%9B%E6%96%B9%E6%B3%95.md)
- sigmoid 和 tanh 为什么会导致梯度消失？
- 一个隐层需要多少节点能实现包含 n 元输入的任意布尔函数？
- 多个隐层实现包含 n 元输入的任意布尔函数，需要多少节点和网络层？
- [dropout 为何能防止过拟合？](https://github.com/buki26/InterviewQuestions/blob/master/answers/dropout%E4%B8%BA%E4%BB%80%E4%B9%88%E8%83%BD%E9%98%B2%E6%AD%A2%E8%BF%87%E6%8B%9F%E5%90%88.md)
- dropout 和 BN 在前向传播和方向传播阶段的区别？

### CNN

- 给定卷积核的尺寸，特征图大小计算方法？
- 网络容量计算方法
- 共享参数有什么优点
- 常用的池化操作有哪些？有什么特点？
- CNN 如何用于文本分类？
- resnet 提出的背景和核心理论是？
- 空洞卷积是什么？有什么应用场景？

### RNN

- 简述 RNN，LSTM，GRU 的区别和联系
- 画出 lstm 的结构图，写出公式
- RNN 的梯度消失问题？如何解决？
- lstm 中是否可以用 relu 作为激活函数？
- lstm 各个门分别使用什么激活函数？
- 简述 seq2seq 模型？
- seq2seq 在解码时候有哪些方法？
- Attention 机制是什么？

## 机器学习

### 基础

- 样本不均衡如何处理？
- 什么是生成模型什么是判别模型？

### 集成学习

- 集成学习的分类？有什么代表性的模型和方法？
- [如何从偏差和方差的角度解释 bagging 和 boosting 的原理？](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E5%AF%B9%E4%BA%8Ebagging%E3%80%81boosting%E5%81%8F%E5%B7%AE%E5%92%8C%E6%96%B9%E5%B7%AE%E7%9A%84%E7%90%86%E8%A7%A3.md)
- GBDT 的原理？和 Xgboost 的区别联系？
- adaboost 和 gbdt 的区别联系？

### 模型

- 手推 LR、Kmeans、SVM
- 简述 ridge 和 lasson 的区别和联系
- 树模型如何调参
- 树模型如何剪枝？
- 是否存一定存在参数，使得 SVM 的训练误差能到 0
- 逻辑回归如何处理多分类？
- 决策树有哪些划分指标？区别与联系？
- 简述 SVD 和 PCA 的区别和联系？
- 如何使用梯度下降方法进行矩阵分解？
- LDA 与 PCA 的区别与联系？

### 特征工程

- 常用的特征筛选方法有哪些？
- 文本如何构造特征？
- 类别变量如何构造特征？
- 连续值变量如何构造特征？
- 哪些模型需要对特征进行归一化？
- 什么是组合特征？如何处理高维组合特征？

## 其他（分方向）

- word2vec 的原理，glove 的原理，fasttext 的原理？
- cbow 和 skipgram 如何选择？
- 了解 elmo 和 bert 吗？简述与 word embedding 的联系和区别
- 图像和文本和语音数据各有哪些数据增强方法？
- rcnn、fatse rcnn、fatser rcnn、mask rcnn 的原理？
- 介绍 resnet 和 GoogLeNet 中的 inception module 的结构？
- 介绍 yolo 和 ssd ？
- 介绍 FM，FFM，deepFM，deepWide.
- 机器翻译如何解决 oov？
