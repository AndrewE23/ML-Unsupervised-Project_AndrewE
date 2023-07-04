# Machine Learning Project: Unsupervised Learning

## Project Outcomes
Unsupervised Learning: Use EDA and different unsupervised learning models to analyse and better understand not only the Wholesale Data dataset, but what insights can be learned from it.

### Setup:
Import libraries and load .csv file; libraries are loaded at the start so that you don’t need to hunt down multiple cells to load them for different components.

### EDA:
Mostly deals with exploring and visualizing data. The assignment was structured in a way where I could do this prior to creating my visualisations and executing models.

### Preprocessing:
The data was relatively clean; we had no NaNs, no 0s as placeholder values, and no duplicates. However, some data was still normalized—especially when it came to outliers. I also hot-encoded a value that did not need to be encoded, "Region", because I wanted to demonstrate knowledge that would have been more beneficial had I needed to bin anything (which I also felt was not necessary to do). Region has little correlation with any other variable, so I felt that further manipulation and use of that variable was not necessary.

### Models:
We utilise K-means clustering, hierarchical clustering, and PCA methods for understanding the data as provided. 

### Conclusion (Findings):
While working with the Wholesale Data dataset, I was able to analyse and model the data to work out the following:
- Correlations:
    - Businesses who buy detergents & paper products also tend to buy a lot of grocery and milk products. 
    - Similarly, there is a mild correlation between fresh and frozen food sales, as well as delicatessen and milk sales. 
    - We have a mild negative correlation between fresh and detergents/paper products, which suggests that clients are less likely to buy both together. There are similarly mild negative correlations for frozen products to grocery products, and for frozen to detergents & paper.
- There are no substantial differences in the purchasing habits of wholesale customers between different regions, meaning that any strategies employed to improve sales should be applicable in any of the three identified regions or region categories.
- Depending on the clustering method used, we can identify 2-4 distinct business clusters from the data. This could allow, for example, marketing or sales strategies to maximize the employer's business operations.
- There are some areas where our two Channels, Ho/Re/Ca and Retail, differ substantially in terms of their buying habits and what they need to conduct business. This could be used to conduct further analyses to figure out exactly how to proceed, but these variances exist and are important to note.

### Small Concerns & Time Issues:
1. I could have scaled the data once, prior to creating any of my three models. I initially did but also wasn't certain if I would have to do anything with the original data, so I elected to copy and transfer that code segment into each model component. See point 2 for further thoughts on this:
2. I also wanted to utilise a pipeline, but again had time constraints given the same-day due date and the fact I still had other school activities to work on. If I revisit this project in the future then I will be creating a class that can be used to scale my data and fit my columns only once, so that each model can simply load the object without having to copy+paste my code over and over again.
  - The same goes for my functions.
  - I may spend my first week post-bootcamp cleaning this and other projects, making them more efficient.
