# Data_Preprocessing_70_80Percent_Work





## Categorical variables

Categorical variables must be converted using either ordinal encoding or one-hot encoding. The former must be used if the categories follow some order, the latter if they don't. If we use a supervised machine learning model that can deal with categorical variables directly, encoding is not necessary.
## Scaling

Scaling must be used only if the model requires scaled data.

If the features have very different variances, you can start with Standardization. If there are too many outliers, you can use Robust Scaling. Otherwise, you can use Normalization.
## Training and test set

Every data pre-processing pipeline used in a supervised machine learning project must be trained only on the training dataset. The trained pipeline can then be used to transform the test set and any other dataset the model will be applied on.
## Feature importance

Feature importance is a very useful technique to filter out unnecessary variables. If you have hundreds of variables, my suggestion is to reduce them to no more than 50 features before applying PCA. If you prefer not to use PCA, my suggestion is to reduce the number of features to no more than 20.
## SMOTE

Always remember to scale your data before applying SMOTE. If the features are very skewed, consider the use of a power transformation.