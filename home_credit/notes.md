# TODO
- Plot each feature, ordered by importance.
  - Compare distribution between positive examples vs negative examples.
  - Compare distribution between training data vs test data.
- Likelihood encoding on categorical features with high cardinality.
  - KFold-mean to avoid overfitting.
- Baysian optimization of hyperparameters.
  - https://www.kaggle.com/willkoehrsen/automated-model-tuning

# Notes
- Even when AUC is the metric, minimizing logloss might be better than minimizing AUC loss.
- Define your goals. What do you want to get from the participation?
  - Choose the right competion to participate.
- Check number of submissions of top people.
  - If many, leaderboard probing.
  - If few, there's some trick few people noticed.
- Check team size of top people.
  - If few, good chance.
- Pickle dataframes. It loads faster than CSV.
  - Pickle is easy.
  - HDF5: df.to_hdf / pd.read_hdf
- Make model overfit once, then tweak regularization to reduce variance.
- Track your code changes so you can reproduce.
- Macro in Jupyter to import common libs.
- Make your own library for frequent operations.
- Reliable validation is the top priority.
- Before reading other people's kernels and discussions, make hypotheses yourself on what could be potentially useful in fresh mind. This makes difference.
- Continue feature engineering until the final week.
- Focus on model selection, hyperparam tuning, ensembling only in the final week.
