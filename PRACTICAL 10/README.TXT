Workflow:
1. Basic Statistics (describe() output)
The describe() table shows the numerical summary of all 13 features in the dataset.
From this output, you can observe:
The mean value of each feature (e.g., average alcohol level).
The standard deviation, showing how spread out values are.
The minimum and maximum values for each column.
The 25%, 50%, and 75% percentiles, which help understand distribution shape.
This table gives a quick overview of the dataset and helps detect outliers or skewed variables.

2. Boxplot by Classes
A boxplot was created for the feature Alcohol across the three wine classes (0, 1, and 2).
From this plot, you can observe:
Each class has a different range and median alcohol level.
Class 1 has generally lower alcohol content, while Class 0 is higher.
The presence of some outliers above or below the whiskers.
This helps understand how features vary between categories and which features might help distinguish classes.

3. Scatter Plot (Alcohol vs Malic Acid)
This plot visualizes the relationship between two features:
Alcohol (x-axis)
Malic Acid (y-axis)
From the scatter plot:
The points show no strong linear correlation, meaning the features vary independently.
The spread of points suggests that some grouping might exist, useful for classification.
This visualization helps identify whether features naturally form clusters.

4. Covariance Matrix Plot
A heatmap of the covariance matrix shows how much each pair of features varies together.
From this output:
Bright (higher) values indicate strong positive covariance (features increase together).
Darker values indicate negative or low covariance.
The feature Proline has high covariance with many other features, meaning it strongly varies with others.
This helps identify which features are strongly related and may influence PCA.

5. Data Scaling Output
After applying StandardScaler, the features are transformed so that:
Mean = 0
Standard Deviation = 1
This ensures all features contribute equally when applying PCA or machine learning algorithms.
Although the scaling itself isn’t shown visually, it affects the PCA output.

6. PCA (Principal Component Analysis) Output
A scatter plot is produced using the first two principal components (PC1 and PC2).
From this PCA plot:
The data points form three visible clusters, representing the three wine classes.
PCA increases the separation between classes compared to raw feature plots.
PC1 and PC2 capture most of the dataset’s variation.
This visualization shows that PCA successfully reduces dimensions while maintaining class separability.

Step	                            Output	What It Shows
1	Describe Table	          Statistical summary of all features
2	Boxplot	                  Difference in feature distribution among classes
3	Scatter Plot	            Relationship between two selected features
4	Covariance Matrix	        Strength and direction of feature relationships
5	Scaling	                  Features normalized for better ML performance
6	PCA Plot	                Improved class separation in 2D space
