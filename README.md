# MNIST

"This project is licensed under the terms of the MIT license."

Msc in Data Science 2020-21, Dimokritos. Machine Learning course. 

In this project we have to process the "MNIST" data set, which has photos with handwritten digits. 
We have to find the best algorithm from a list of algorithms of our choice. 
Below we list the statistics and performance of each of the algorithms we chose for this classification problem.


We run the algorithms, and the measurements with the scaled data of 784 dimensions are shown in the table.
Model	                     hyperparams	                                  Time (sec)	   Accuracy
Decision Tree	             'entropy', max_depth=14	                      6.667	         0.857
Logistic Regression	       solver='lbfgs'	                                13.129	       0.900
K-Nearest Neighbors	       n_neighbors=3	                                2517.461	     0.934
Support Vector Machines	   C=10, kernel='rbf', gamma='auto'	              753.307	       0.964
Naive Bayes.                               -                              5.351     	   0.522
Random Forest	             estims=1000, max_feats=5	                      91.538	       0.960
AdaBoost	                 n_estimators=500	                              417.645	       0.695
XGBoost	                   use_label_encoder=False, eval_metric='error'	  508.168	       0.969



Then, we run the same algorithms with PCA and X_reduced data, which has 154 dimensions.
Model	                      hyperparams	                                  Time (sec)	  Accuracy
Decision Tree	             'entropy', max_depth=14	                       12.608	        0.817
Logistic Regression	        solver='lbfgs'	                               2.309	        0.915
K-Nearest Neighbors	        n_neighbors=3	                                 578.864	      0.883
Support Vector Machines	    C=10, kernel='linear', gamma='auto'	           286.106	      0.967
Naive Bayes	                           -	                                 0.802	        0.856
Random Forest	              estims=200, max_feats=5	                       36.372	        0.935
AdaBoost	                  n_estimators=200	                             138.282	      0.686
XGBoost	                    use_label_encoder=False, eval_metric='error'	 501.507	      0.954


