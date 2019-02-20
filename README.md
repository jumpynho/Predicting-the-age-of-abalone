# Predicting the age of abalone
Predicting the age of abalone using RapidMiner.

This is a building of a classification model of the abalone's age.
In particular, we wanted to identify the best classification model between:
- k-NN
- Decision Tree

It has been shown that k-NN with k = 24 is the best classifier.

### Data pre-processing
The dataset has been subjected to a normalization phase, as the features have different units of measurement.
Furthermore, an outlier detection and removal was carried out.

### Class generation
Based on the value of the Rings attribute, 3 classes have been defined for the age of the abalone:

* Class 1 (Child) - Rings between 0 and 8
* Class 2 (Medium age) - Rings between 9 and 14
* Class 3 (Adult) - Rings greater than 14

## Running the model construction
Import the `model_abalone.rmp` file in your RapidMiner.

Then in Normalization subprocess, import the excel file `abalone.xlsx`.

In 'Write Model' operator set your output location.

Finally, start the process.

If you want create your own classification model you have to loop parameter of the various classifiers.
