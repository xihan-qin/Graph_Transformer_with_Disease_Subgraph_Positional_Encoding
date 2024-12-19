## Graph Transformer with Disease Subgraph Positional Encoding
In this study, we introduced Transformer with Subgraph Positional Encoding (TSPE) for disease comorbidity prediction, inspired by insights from BSE. TSPE leverages Transformer’s attention mechanism to capture node interactions and integrates Subgraph Positional Encoding (SPE) method for disease association information. Node2Vec was utilized for generating node embeddings. Given the skewness in both benchmark datasets RR0 and RR1, we evaluated TSPE's performance using ROC AUC as the primary metric, which is well-suited for skewed datasets, and accuracy metrics as a secondary measure. TSPE demonstrated substantial improvements over the state-of-the-art BSE method with SVM classifier, achieving a 29.84% increase in ROC AUC and a 6.67% increase in accuracy for RR0, with average scores of 0.9649 for ROC AUC and 0.9345 for accuracy. For the RR1 benchmark dataset, TSPE showed a 15.86% increase in ROC AUC and a 5.17% increase in accuracy compared to the state-of-the-art, achieving scores of 0.8055 for ROC AUC and 0.7318 for accuracy.

### TSPE Framework
![fig1](https://github.com/xihan-qin/Graph_Transformer_with_Disease_Subgraph_Positional_Encoding/blob/main/figs/TSPE_framework.png)

### Subgraph Positional Encoding (SPE)
![fig2](https://github.com/xihan-qin/Graph_Transformer_with_Disease_Subgraph_Positional_Encoding/blob/main/figs/SPE.png)

### Results Showcase
#### TSPE vs the State-of-the-Art for Commorbidity Prediction
Bechmark Datasets: RR0 and RR1.
<table>
<thead>
  <tr>
    <th rowspan="2">Metric</th>
    <th colspan="3">RR0</th>
    <th colspan="3">RR1</th>
  </tr>
  <tr>
    <th>SVM</th>
    <th>BSE_SVM</th>
    <th>TSPE</th>
    <th>SVM</th>
    <th>BSE_SVM</th>
    <th>TSPE</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>roc_auc</td>
    <td>0.5309</td>
    <td>0.6665</td>
    <td><strong>0.9489</strong></td>
    <td>0.5497</td>
    <td>0.6469</td>
    <td><strong>0.8009</strong></td>    
  </tr>
  <tr>
    <td>Accuracy</td>
    <td>0.8357</td>
    <td>0.8765</td>
    <td><strong>0.9069</strong></td>
    <td>0.6150</td>
    <td>0.6801</td>
    <td><strong>0.7294</strong></td>              
  </tr>
</tbody>
</table>

#### SPE Ablation Analysis
NoPE: no positional encoding; LPE: a popular positional encoding proposed in Dwivedi et al.'s work; SPE: our subgraph positional encoding
<table>
<thead>
  <tr>
    <th >Metric</th>
    <th >NoPE</th>
    <th >LPE</th>
    <th >SPE</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>roc_auc</td>
    <td>0.7971</td>
    <td>0.8007</td>
    <td><strong>0.8009</strong></td>
  </tr>
  <tr>
    <td>Accuracy</td>
    <td>0.7214</td>
    <td>0.7234</td>
    <td><strong>0.7294</strong></td>            
  </tr>
</tbody>
</table>

### Note
For additional details, please consult the paper titled "Graph Transformer with Disease Subgraph Positional Encoding  for  Improved Comorbidity Prediction."
