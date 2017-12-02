# ch2 模型评估与选择

## 性能度量

得到的模型需要一些评估好坏的指标。我们先在测试集上评估而不考虑泛化能力。  
这里讨论二分类任务。
- 错误率与精度：错误率=分类出错的/测试集规模，精度=1-错误率    
- 查准率（precision）查重率（recall和F1：首先明确混淆矩阵的概念（TP,FP,TN,FN）。  
	- 查准率：选出来的有多少是真的好 $P = TP/(TP+FP)$  
	- 查全率：好的有多少被选出来 $R=TP/(TP+FN)$
	- F1：为什么定义F1，我们希望P和R都好，二者之间需要tradeoff。F1是P,R调和平均。
	- $F_\beta$：有时我们P和R不是同样重要的，于是加权调和平均。   
	- 多个测试集上的多个混淆矩阵：macro-, micro-
- ROC（receiver operating characteristic）与AUC（area under curve）  
	- 

