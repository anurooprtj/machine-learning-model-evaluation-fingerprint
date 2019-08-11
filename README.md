# machine-learning-model-evaluation-fingerprint
Performance comparion of various machine learning models on background and foreground classification for fingerprint data.

### Dataset creation

1. 50 fingerprint images were used to create the dataset. 
2. From each image 5 pathches for foreground and background were selected having length 21X21.
3. GLCM properties were applied on each fingerprint patch:
	- contrast
    - dissimilarity
    - homogeneity
    - energy
    - correlation
    - ASM
4. Class label 1 for foreground and class label 0 for background assigned. 
5. fingerprint.csv file created.
6. fingerprint_pickle file is used to read created fingerprint.csv file, Create X, y, standardize (Standard scalar) them and diviee into training and testing data.  

### Machine learning models used:
1. Logistic regression
2. Support Vector Machines - linear and rbf
3. Decision Trees
4. Random Forest
5. Adaboost classifier
6. Gradient boost classifier

### Model Selection

Except for Logistic regression, best model for each machine learning method is selected using hyperparameter tuning.

### Evaluated results for each model

1. Cross validation score
2. Mean score
3. Standard deviation
4. Confusion matrix
5. Precision, Recall and F1 score

### Performance Chart 

![alt text](https://github.com/anurooprtj/machine-learning-model-evaluation-fingerprint/blob/master/model_comparison_chart.png)