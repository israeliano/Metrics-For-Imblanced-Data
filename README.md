# Metrics For Imblanced Data

(there is a typo: FNR should be TNR)

Which metric is best suited if the data is imbalanced? We compare area under the receiver operating characteristic curve (`ROC-AUC`), the area under the Precision-Recall curve (`PRC-AUC`) and $F_1$-score (`F1`) for imbalanced data.

The clusters to be studied have $10^3$, $10^4$ and $10^5$ points and an imbalanced of $0.5$ (balanced), $0.75$, $0.9$ and $0.99$:

![Clusters](https://github.com/israeliano/Metrics-For-Imblanced-Data/blob/main/clusters.png)

Using XGBClassifier, we see how the metrics change when the predictions change:

![Metrics Behaviour](https://github.com/israeliano/Metrics-For-Imblanced-Data/blob/main/metrics.png)

We see clearly that both the `F1` and `PRC-AUC` decrease as the Precision and Recall decrease.
