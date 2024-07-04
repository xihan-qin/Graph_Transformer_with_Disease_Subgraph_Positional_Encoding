# Graph Transformer with Disease Subgraph Positional Encoding
In this study, we introduced Transformer with Subgraph Positional Encoding (TSPE) for disease comorbidity prediction, inspired by insights from BSE. TSPE leverages Transformer’s attention mechanism to capture node interactions and integrates Subgraph Positional Encoding (SPE) method for disease association information. Node2Vec was utilized for generating node embeddings. Given the skewness in both benchmark datasets RR0 and RR1, we evaluated TSPE's performance using ROC AUC as the primary metric, which is well-suited for skewed datasets, and accuracy metrics as a secondary measure. TSPE demonstrated substantial improvements over the state-of-the-art BSE method with SVM classifier, achieving a 29.84% increase in ROC AUC and a 6.67% increase in accuracy for RR0, with average scores of 0.9649 for ROC AUC and 0.9345 for accuracy. For the RR1 benchmark dataset, TSPE showed a 15.86% increase in ROC AUC and a 5.17% increase in accuracy compared to the state-of-the-art, achieving scores of 0.8055 for ROC AUC and 0.7318 for accuracy.

#  Results Showcase
For additional details, please consult the paper titled "Graph Transformer with Disease Subgraph Positional Encoding  for  Improved Comorbidity Prediction."

### TSPE Framework
![fig1](https://github.com/xihan-qin/Graph_Transformer_with_Disease_Subgraph_Positional_Encoding/blob/main/figs/TSPE_framework.png)

### SPE 
![fig2](https://github.com/xihan-qin/Graph_Transformer_with_Disease_Subgraph_Positional_Encoding/blob/main/figs/SPE.png)