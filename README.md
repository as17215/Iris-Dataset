Exploring the iris dataset and generating a predictive model to determine iris species

Background

Iris is a flowering plant and the common name given to all iris species. A famous dataset which took 50 samples of each of the three species: setosa, versicolor and virginica, is outlined in Fisher's paper. It collects data on the sepal length and width and petal length and width. The aim of the code produced uses k-nearest neighbours (kNN) and principal components analysis (PCA) to define boundaries between the species to form a model that can predict the species of iris with good confidence given the features described above.

Methods & Results

The code looks at the correlation between the four features to see what is going on and what trends are present. It then uses the most uncorrelated pair to base the kNN model on to define the boundaries between the three species and nearest neighbour classification using machine learning. The StandardScaler funciton is used to scale the data and thus, provide an even distribution. PCA is also employed to reduce dimensionality and improve the model score whilst accounting for a vast amount of variation in the data. This makes it a more realistic model which represents the data as a whole, generating a successful predictive model for determining the species of iris.

Conclusion

In conclusion, the final model had a score of 0.95 and is a good predictor for species of iris. It is important to note that setosa is well separated from versicolor and virginica whereas, there is overlap between versicolor and virginica.

Running the code

1. First download all the files in this repository into a single directory. This should include the main code (iris_species_predictor.ipynb), the plot module (plot.py), the README file (README.md) and the picture (iris_picture.jpg). 

2. The second line of code requires you to copy the path for the iris_picture.jpg downloaded in your directory and paste it in-between the inverted commas to enable the relavent image to be inserted into the notebook

3. All the code can then be run (All the relavent modules that need to be imported are embedded throughout the code. No external modules need to be imported to Juypter lab.)

The code should have now run smoothly producing all the relavent outputs and graphs. The final model score should have been 0.947 (3 d.p.).

Note: If warning messages in red boxes show up in the notebook once the code has been run then copy the lines of code below at the start of the notebook and restart the kernel and re-run all the code. This should get rid of any red warning messages that showed up previously.

Code:

import warnings warnings.simplefilter(action='ignore', category=FutureWarning) 