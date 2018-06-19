- Remove outliers from training data set
  - They don't add value to the model.

- XGBoost outputs feature importance.
  - For each important feature, visualize distribution and correlation with the label.
  - Find and eliminate outliers.
  - Consider binning
  - Consider normalization
  - Consider log1p transformation to make a long-tail curve closer to a symmetric bell curve.
  - Remove unimportant features to generalize better.

- Think about relation among data points.
  - Maybe try to cluster by family. Families maybe share consequences.

- Add a column for null vlaue count.
  - Quantifies the amount of information each data point has.

- Guess null values from other features.
  - e.g. Guess age from pclass and sex.

- Categorical variables: consider one-hot encoding.

- Grid search
  - Use separate validation data set for CV, to avoid overfitting to the data set.

- Cross Validation
  - Find the number of kfold such that local CV score matches the public leaderboard score.

- Avoid overfitting: Regularization
  - Suppress high variance by increasing regularization term.
  - It's easier to control regularization than number of features when ensembling many models.

- Pandas
  - df.sample(frac=1)
    - random shuffle. https://stackoverflow.com/questions/29576430/shuffle-dataframe-rows
  - pd.concat()
    - axis=0 concatenates vertically
    - axis=1 concatenates horizontally
  - pd.get_dummies()
    - categorical => one-hot
  - pd.cut() and pd.qcut()
    - binning

- Seaborn
  - plot and grid
  - two-color pallete for correlation matrix.

- Helpful Kernels
  - https://www.kaggle.com/startupsci/titanic-data-science-solutions
  - https://www.kaggle.com/helgejo/an-interactive-data-science-tutorial
  - https://www.kaggle.com/jeffd23/scikit-learn-ml-from-start-to-finish

- Helpful webpages
  - https://github.com/nejumi/kaggle_memo
  - https://mlwave.com/kaggle-ensembling-guide/

