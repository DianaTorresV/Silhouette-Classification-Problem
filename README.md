---
# Vehicle Classification Using Geometric Features

## Repository Overview

This project employs supervised machine learning techniques to classify vehicles into three categories—bus, car, and van—using geometric features extracted from their silhouettes. It serves as an introductory, hands-on exercise in applying machine learning concepts to solve real-world-like problems.

Developed as part of the Data Analytics & Science program at Masterschool, this first machine learning project reflects a personal approach to the solution, independent of the program's specific curriculum. The project emphasizes mathematical reasoning and structured analysis, ensuring a logical and systematic problem-solving framework.

In this repository, you will find:
* PDF documentation detailing the project.
* A Colab notebook outlining the process and methodology.
* The dataset in a CSV file.

### Motivation and Context
The motivation behind this project is to gain hands-on experience with supervised machine learning algorithms and data analysis techniques. By addressing a practical classification problem, the project emphasizes applying foundational knowledge to uncover insights and build predictive models.

The project was completed within a limited three-day timeframe and is framed as a foundational exercise to bridge basic machine learning concepts with real-world applications.

### Technologies and Tools
The project utilizes the following technologies and libraries:

* Python
* Google Colab
* Libraries:
  * Pandas: Data manipulation and cleaning.
  * Matplotlib & Seaborn: Visualization of distributions and feature separability.
  * Scikit-learn: Model building, tuning, and evaluation.


### Problem Description

A chain of car repair shops, "Prospect Auto," seeks a machine learning model to classify vehicles—bus, car, and van—based on their silhouettes. Using a dataset comprising geometric features, the goal is to develop and evaluate a classification model capable of distinguishing between the three vehicle types.

### Data Summary
The dataset consists of numeric features describing geometric aspects of vehicle silhouettes:

* **Class distribution:** 218 buses, 429 cars, and 199 vans (slight imbalance).

* **Features:** All numerical, representing ratios, dimensions, and aspect-based measures of vehicle geometry.

* **Data quality:** Minimal missing values (<1%), addressed through mean imputation.
  
### Process and Methodology
* **Data Preprocessing**
  * Scaled features using StandardScaler to ensure compatibility with linear models.
  * Explored log transformation for selected features but retained original values for better performance. 
* **Exploratory Data Analysis (EDA)**
  * Univariate Analysis: Highlighted features like compactness with strong class separation.
  * Bivariate Analysis: Identified high correlations (>95%) between some features, particularly affecting linear models.
  * Visualized data using histograms, KDE plots, and boxplots to detect skewness, outliers, and potential separability.
* **Model Building**
  * Logistic Regression: Achieved 93.5% accuracy with StandardScaler. Experimented with log transformations but retained raw scaling for optimal results.
  * Decision Tree: Tuned max_depth (optimal depth = 10). Provided basic interpretability but underperformed compared to other models.
  * Random Forest: Achieved the highest accuracy (98.2%) with 50 estimators. Robust against skewness and multicollinearity.Revealed important features driving classification accuracy.

### Limitations
* Classification relied exclusively on geometric data, restricting the scope of the model.
* Only three machine learning algorithms were explored, with optimization performed manually.
* The project inspired further study of more advanced tools and techniques, highlighting opportunities to explore complex methodologies for improving performance and achieving better optimization.

-----

