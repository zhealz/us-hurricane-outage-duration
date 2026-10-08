# Check with scikit-learn 1.9.1

The same `step4_modeling` notebook and the same input tables, run with scikit-learn 1.9.1 instead of 1.6.1 (Python 3.13, numpy 2.5, pandas 3.0). Only the gradient-boosted-tree results differ; the ridge results are identical.

The gains under the strict test can be recomputed from the `strict_*` columns of `step4_predictions.csv`: the Spearman correlation with `hours_above` inside each hurricane, averaged over the nine.
