
Model Comparison Report for Bank Marketing Campaign
---------------------------------------------------

Our Objective was to identify best machine learning classification model which can predict the customer buying the term deposit with the aim to find as many buyers possible who can be potential customers while utilizing the marketing resources most effectively to minimize spending them on people not likely to buy.

We ran multiple classification models to compare the Accuracy, Precision, Recall and Training time to generate the above comparison table. Since the target classes are very unbalanced in the given dataset given yes 14% to no 86%, the accuracy may not the very reliable metric for decision making. We need to look at Precision and Recall which provides a better insight in the performance of the model. Looking at the table which shows the results from the different classification models here are the key findings and model performance comparison in details.

Key Findings
------------

- If the marketing strategy is to target the buyers with the most likelihood of making purchase, than DecisionTreeClassifer model is most suitable 	since it has the highest Precision rate of 50% which means out of every 2 calls, one call gets converted in success. However the Recall is 35%   which means it is only able to find only 35% of the potential buyers. So this model is suitable for the scenario where the marketing strategy is to quickly target the most likely customers by allocating the minimum resources or with small merketing team.
- If the marketing strategy is to target the broader market and find as many potential customers as possible, then LogisticRegression provides a more balance between Recall and Precision. With Recall of 56%, it is able to find 56% of potential buyers much higher than 35% as discovered by DecisionTreeClassifier model. This provides a much bigger pool of potential customers for marketing team. However the Precision is 31% which means that only one in three calls will convert in success. So this model is more suitable for broader search for potential customers when more budget and bigger marketing team is available.
- The given dataset is not a good fit for KNN model. The Training accuracy of 99% indicates overfitting and does not perform well with the test data. Though it has a decent precision of 40% but the recall is very low at 23%. Also the model is slow and has a much higher training time compared to other models except SVC-rbf.
- LinearSVC can be a good alternative to Logistic Regression given almost comparable performance of both the models.
- SVC-rbf provides a good balance of Precision 40% and Recall 50%, however it is extremely slow compared to the other models and show it is computationaly very expensive to operate without providing any major benefit over other models.