# AliCould_Game_Happiness

## Tips
* 似乎特征工程用处不是很大；
* 对数据标准化会比较有用，例如：最大最小正则化，Z-Score标准化，归一化；对于logistic Regression使用标准化，准确率会有2~3%的提升；
* 交叉验证也比较有用，KFold：对于Logistic Regression使用15折KFold，在测试集中MSE升高了0.0072；提交到网页发现：不使用KFold,MSE:0.60991;使用KFold,MSE:0.59238;发现使用KFold,MSE降低0.01753
* LightGBM的相对于Logistic Regression的提升很巨大，均使用15折KFold，Z-Score标准化，简单的特征工程：LC的MSE是0.59238，LGBM的MSE是0.48282，发现提升巨大。

由上可以看出，对于幸福感这个赛题，使用更好的算法，结果提升很大<br>
## 常用的分类模型的优劣点及常用场景；




## 优化方法
* GrindSearch：https://blog.csdn.net/weixin_41988628/article/details/83098130
* 在sklearn的中：from sklearn.model_selection import GridSearchCV

## Stacking
* Stacking的机制类似于人民代表大会机制
*
