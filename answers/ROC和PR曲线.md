# ROC 和 PR 曲线

## ROC 曲线

ROC 曲线，形如：
![ROC曲线](https://github.com/buki26/image/blob/master/AUC%E6%9B%B2%E7%BA%BF.jpg?raw=true)
横坐标 FPR，纵坐标 TPR
要理解 FPR 和 TPR，首先看混淆矩阵，混淆矩阵由 TP、TN、FP、FN 组成
T 和 F 可以理解为预测正确与否（true 和 false）
P 和 N 可以理解为预测为正例或预测为负例（positive 和 negative）
例如 FP 就是实际为负例被预测为正例的样本数

从上面的定义中可以得到的信息是，实际为正样本的数量为（TP+FN），实际为负样本的数量为（TN+FP）

FPR——False positive rate,实际为负样本中被预测为正样本的概率，FPR=FP/(TN+FP)
TPR——True positive rate,实际为正样本中被预测为正样本的概率，TPR=TP/(TP+FN)
以 FPR 和 TPR 作为横坐标和纵坐标画出的评价模型的曲线就叫做 ROC 曲线

由于以曲线作为评价标准不好衡量和对比，引入 AUC (Area Under Curve),是一个值，这个值等于 ROC 曲线下的面积，越大说明模型越好
如图所示：
![AUC](https://github.com/buki26/image/blob/master/AUC.jpg?raw=true)
另外一点需要注意的是，如下图，两个模型的 ROC 曲线如下图，假设 AUC 值相等的话，并不能代表这两个模型效果一样，因为侧重点不同
![相等的AUC](https://github.com/buki26/image/blob/master/%E7%9B%B8%E7%AD%89AUC%E5%80%BC.jpg?raw=true)

## PR 曲线

这里的 PR 指的是 precision 和 recall，也就是准确率-召回率曲线，形如：
![PR曲线](https://github.com/buki26/image/blob/master/PR%E6%9B%B2%E7%BA%BF.jpg?raw=true)
横坐标 recall，纵坐标 precision
recall,实际为正样本中被预测为正样本的概率（和 TPR 是一样的），recall=TP/(TP+FN)
precision，只针对正例的准确率，也就是所有预测为正的样本中，预测正确的，precision=TP/(TP+FP)
