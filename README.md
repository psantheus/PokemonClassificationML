# PokemonClassificationML
A simple project to predict what pokemon is given as input to a trained model.
Various Machine Learning Algorithms have been used and discussed below.

## Dataset Used
[Link to Dataset](https://drive.google.com/file/d/1pJS6erT9C7fgdE76bR2Dp6LIw2Goe7cU/view?usp=sharing)

Dataset consists of 5 classes, each filled with 280 images.
The data was split manually into training and testing data so that each class is present equally in both sets of data.
For the sample results below, a train-test split ratio of 3:1 was used.

## KNN
KNN or K nearest neighbors is a non-parametric classification method that can be used for both classification and regression problems. There is no particular training involved, all computation is put on hold until the query is made. The basic theory is that, KNN looks for the "k closest neighbors" by distance between the input and the "training set", and applies majority voting on those to decide what class does the input belong to.

![KNN-embed](https://i.imgur.com/6XsPdfc.png)

For the above example, for K = 4, Red is in the majority compared to Blue, and input gets predicted as Red. For K = 7 on the other hand, Blue outnumbers Red, and input gets predicted as Blue instead.

One of the drawbacks of KNN is when the classes are largely unbalanced. Using the uniform KNN results in a skewed prediction since one of the classes is in the majority for a range of values of K. A workaround is to use weighted KNN instead, which considers the closest neighbors to have more weight than the farther ones, this clears up some skewness that was coming from a numerical advantage.

Obtained a validation accuracy of 65.4% on the uniform KNN and a validation accuracy of 71.1% on the weighted KNN.

# Logistic Regression
Obtained validation Accuracy of 82.8%

# Naive Bayes
Obtained validation Accuracy of 49.4%

# Support Vector Machines
Obtained validation Accuracy of 84.8%

# Convolution Neural Networks
Obtained validation Accuracy of 83.4%
