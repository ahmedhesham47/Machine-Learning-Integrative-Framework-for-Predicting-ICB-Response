# Machine-Learning-Integrative-Framework-for-Predicting-ICB-Response
A Machine Learning project that aims to predict the response to ICB therapy using integrative data sources --> Clinical, Gene Expression, Gene Single Nucleotide Polymorphism Mutation, and Gene Copy Number Alteration Mutation.

We implemented 6 feature selection methods to choose the best response-associated genes in the gene expression and mutation datasets. They are FDR, correlation, recursive feature elimination, select from model, random forest, and gradient boost. We chose the 5 combinations that led to the highest number of intersecting genes.
However, we also tested another hypothesis, which is whether genes selected from the gene expression matrix (let them be called transcriptomic-response associated genes) can also discriminate responders from non-responders in the mutation datasets.

As the results show, this hypothesis was refuted. It is better to select the best response-associated genes from each dataframe separately; that is, transcriptomics-response-associated genes are NOT ALSO mutation-response-associated.

To test this hypothesis, we implemented 3 classifiers, Random Forest, Support Vector Machine, and Logistic Regression, on two datasets: Liu and Ravi. All the needed data can be found in the Data directory. The results can be found in the Outputs directory.

To run the code, just import the packages and files of your desired dataset (Liu or Ravi), and run the code sequentially.
