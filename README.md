# GameSalesMLProject
Game Sales Machine Learning Project

Introduction

The video game industry generates a massive amount of data, ranging from game titles and genres to sales figures in different regions worldwide. Analyzing this data can provide valuable insights into market trends, player preferences, and sales patterns, which can be leveraged for strategic business decisions. This project focuses on analyzing a Game Sales Dataset, aiming to predict and classify sales figures, as well as discover inherent patterns in the data through clustering.
The project is divided into three main categories: Regression, Classification, and Clustering. Each section is designed to address a unique analytical goal, using various machine learning models and evaluation techniques. By breaking down the dataset into these categories, we aim to not only predict sales but also classify outcomes and segment data for deeper insights. 

The entire workflow begins with data preprocessing, ensuring the dataset is clean, reliable, and free of errors that could impact the models' performance.

1. Data Preprocessing: Before diving into modeling, data preprocessing is crucial to ensure clean and accurate data for analysis. The preprocessing steps taken in this project include:

•	Handling Missing Values: Missing data was addressed using imputation techniques to ensure the dataset is complete.

•	Outlier Detection and Treatment: Outliers, which could distort the results, were identified and either removed or adjusted to prevent them from skewing the data.

•	Data Augmentation: Techniques were applied to enrich the dataset and increase the robustness of the models, particularly when dealing with limited data.
These preprocessing steps ensure the dataset is ready for the next stages of analysis.

2. Regression Models

•	Objective: To predict Global Sales using various regression models. The target variable is global sales, and the goal is to implement multiple models and compare their performance.


•	Models Implemented:

o	Linear Regression

o	Gradient Boosting Regressor

o	Ridge Regressor

o	Random Forest Regressor


•	Evaluation Metrics: The performance of each regression model was evaluated using the following metrics:

o	Mean Absolute Error (MAE): Measures the average magnitude of errors in predictions.

o	Mean Squared Error (MSE): Penalizes larger errors more than smaller ones by squaring the differences between actual and predicted values.

o	R-Squared (R²): Indicates the proportion of the variance in the dependent variable that is predictable from the independent variables.

o	Adjusted R-Squared: Similar to R² but adjusts for the number of predictors in the model.

o	Accuracy: Used to assess how close the predicted values are to the actual values 

•	Feature Importance: After identifying the best-performing model, feature importance was plotted to show which features (such as genre, region sales, rating, etc.) contribute the most to Global Sales. This visualization helps in understanding the most impactful variables driving game sales globally.


3. Classification Models

•	Objective: To classify various game-related outcomes using 

•	classification models: This part of the project focuses on categorizing the dataset based on different target variables (such as genre, platform and rating) and predicting these categories using machine learning algorithms. Then compare which target variable best classify the dataset.

•	Model Implemented: Gradient Boosting Classifier

•	Implementation: The Gradient Boosting Classifier was applied multiple times with different columns from the dataset as the target variable. This allowed for experimentation in classifying various aspects of the dataset, providing insights into the relationships between features and classification outcomes. The classification model’s performance was evaluated using relevant metrics such as accuracy, precision, recall, and F1-score.


4. Clustering Models

•	Objective: To identify natural groupings or clusters within the dataset, which can provide insights into hidden patterns and relationships between data points, such as games with similar sales trends across different regions.

•	Methodology: Elbow Method used to determine the optimal number of clusters. This technique helps identify the point at which adding more clusters does not significantly improve the model, thus balancing complexity and interpretability.

•	Clustering Evaluation Metrics: To evaluate the quality of the clusters, multiple metrics were used, including:

o	V-measure Score: A harmonic mean of homogeneity and completeness, indicating how well the clustering partitions the data.

o	Adjusted Rand Index (ARI): Measures the similarity between predicted and actual clusters, adjusted for chance.

o	Adjusted Mutual Information (AMI): A measure of the agreement between two clusterings, adjusting for chance.

o	Davies-Bouldin Score: Assesses the quality of clustering based on intra-cluster similarity and inter-cluster differences (lower values are better).

o	Silhouette Score: Indicates how similar a data point is to its own cluster compared to other clusters.

o	Calinski-Harabasz Score: Evaluates the ratio of the sum of between-cluster dispersion and within-cluster dispersion (higher values indicate better clustering).
These metrics ensure that the clustering model not only groups data effectively but also provides meaningful and interpretable results.


5. Conclusion

In this project, we explored the Game Sales Dataset using various machine learning techniques in three key areas: regression, classification, and clustering. The preprocessing stage ensured a clean and robust dataset, while the regression models provided insights into the factors influencing global sales. The classification models allowed for the prediction of game categories, and the clustering models revealed natural groupings within the data.
By evaluating the models using multiple performance metrics, we ensured that the most effective methods were identified and implemented. The findings from this project can be used to make data-driven decisions, predict future game sales, classify games based on key features, and discover hidden patterns within the gaming market.
This README file provides a comprehensive overview of the steps taken in this project and serves as a guide for understanding the data, models, and results.
