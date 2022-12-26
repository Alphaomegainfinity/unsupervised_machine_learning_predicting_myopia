# Myopia Clusters

Using unsupervised machine learning to fit data into a model and using clustering algorithms to place data into groups. Then, create a visualisation to display a trend. 

## Background

As part of the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. The team has tried—and failed—to improve their classification model when training on the whole dataset. However, the team believe that there might be distinct groups of patients that would be better to analyse separately. So, the supervisor has asked to explore this possibility by using unsupervised learning with provided raw data

## Instructions

This activity is broken down into four parts: 

* Part 1: Prepare the Data

* Part 2: Apply Dimensionality Reduction 

* Part 3: Perform a Cluster Analysis with K-means

* Part 4: Make a Recommendation 

### Part 1: Prepare the Data

1. Read `myopia.csv` into a Pandas DataFrame.

2. Remove the "MYOPIC" column from the dataset.

    * **Note:** The target column is needed for supervised machine learning, but it will make an unsupervised model biased. After all, the target column is effectively providing clusters already! 

3. Standardise the dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

### Part 2: Apply Dimensionality Reduction

1. Perform dimensionality reduction with PCA. Is there any changes in the number of the features?

  For this project, preserve 90% of the explained variance in dimensionality reduction.

2. Further reduce the dataset dimensions with t-SNE and visually inspect the results. Using the output of the PCA transformation when running t-SNE on the principal components

3. Create a scatter plot of the t-SNE output. Checking any distinct clusters

### Part 3: Perform a Cluster Analysis with K-means

Create an elbow plot to identify the best number of clusters.

* Use a `for` loop to determine the inertia for each `k` between 1 through 10. 

* Determine where the elbow of the plot is, and at which value of `k` it appears.

### Part 4: Make a Recommendation

Write up a brief (one or two sentences) recommendation for your supervisor whether the patients can be clustered. If so, into how many clusters? 


## References

Reduced dataset from [Orinda Longitudinal Study of Myopia conducted by the US National Eye Institute](https://clinicaltrials.gov/ct2/show/NCT00000169)

- - -

© 2022 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.