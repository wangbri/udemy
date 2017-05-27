# Section 2
## ML Algorithms and Datatypes
*using (ml_algorithm_intro_and_datatypes.ipynb)*

- Use df.**corr()** to initially look for possible correlations/linear relationships in the data.
- Use df['count'].**describe()** for viewing information (mean, std, distribution) about numerical data.
- Use df.seasons.**value_counts()** for viewing information (# of instances) about categorical and binary data.

Labeled data contains the features and target attributes for a dataset and the correct answer for each example. Will want to reserve ~70% of labeled data for training the model and ~30% to verify the prediction quality of the model. AWS tokenizes text input at whitespaces. Categorical data is used for fixed sets of values and numerical data is for finding measurements.

### Binary Classification
Predict a binary class as output based on given features. Also gives a confidence score based on the 0-1 output (such as 70% confidence for output of 1). (e.g. presence of diabetes)

When given training data for detection of health conditions, typically given a lot of normal example and very few "positive" examples where the condition is present.

### Multiclass Classification
Predict a class as output based on given features. (e.g. type of Iris plant)

---

## Data Visualization
*using (ml_plot_types.ipynb)*

- Use df.index.**map(lambda x: x*x)** to map all values from df.index to an array containing the outputs of the mapping function specified in the params.
- Use indices in the dataframe as inputs for the dataset and map it an output using the mapping function.
