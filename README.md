##Course code and title: COMP5200M 
##MSc project Malware Detection

##Requirement
-python                    3.8.13 
-gensim                    3.7.2
-pandas                    1.4.3
-xgboost                   1.5.0
-jupyter_core              4.10.0 
-networkx                  2.8.4 
-numpy                     1.22.4  
-tqdm                      4.64.0 



##Run Configuration: GPU/CPU


##Python packages:

jupyter notebook

Chongxin34.csv - feature importance （5-folded）

Original4.csv - online test submission 

##Parameters of the XGBoost
'max_depth': 6
'eta': 0.01
'eval_metric': 'mlogloss'
'silent': 1
'objective': 'multi:softprob'
'num_class': 8
'subsample': 0.9
'colsample_bytree': 0.85



##The structure of the system:

#Feature Extraction

First-order Statistical Features
Higher-order Statistical Feature
Word2vec 
TF-IDF
ProNE

#Train Model
XGBoost + 5-Folded Cross-Validation



##The output of the logloss

Procedure	Train logloss		Vail logloss
Fold1		0.06141			0.36558
Fold2		0.05049			0.35927
Fold3		0.06019			0.34140
Fold4		0.04974			0.33494
Fold5		0.05521			0.35767


##The result submit to the Alitianchi competition.
online test ： 0.585814

##Reference：
ProNE ：https://github.com/THUDM/ProNE/blob/master/proNE.py author：lykeven
