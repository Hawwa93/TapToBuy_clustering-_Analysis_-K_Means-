## TapToBuy_clustering-_Analysis_-K_Means-
This project focuses on performing customer segmentation using clustering techniques on the TapToBuy dataset. 
The goal is to identify distinct customer groups based on their demographics, lifestyle, and shopping behaviors
to enable more personalized marketing strategies and product recommendations.

## Dataset
- The dataset TapToBuy.csv contains the following customer attributes:
- Age, Gender, Ever_Married, Graduated, Profession, Work_Experience, Spending_Score, Family_Size, Project Workflow

## Data Loading & Cleaning
- Read the dataset using pandas.
- Handled missing values:
- Numeric columns: filled with median.
- Categorical columns: filled with mode.
- Removed duplicates.

## Exploratory Data Analysis (EDA)
- Univariate analysis (histograms, boxplots).
- Bivariate analysis (scatter plots).
- Distribution plots for categorical features.

## Preprocessing
- Scaled numerical features using RobustScaler.
- Encoded categorical variables with LabelEncoder.

## Clustering (KMeans)
- Applied KMeans on:
- Full dataset (scaled + encoded).
- Numeric features only.
- Used Elbow Method and Silhouette Score to find optimal k.
- Performed dimensionality reduction using PCA for 2D visualization.

## Cluster Profiling
- Assigned cluster labels to customers.
- Created a Segment label (e.g., Budget Customers vs Premium Customers).
- Visualized cluster composition and relationships with customer attributes.

## Visualizations
- I created an Elbow Curve and Silhouette Scores to determine optimal clusters.
- 2D PCA Scatterplots of clusters.
- Pairplots to analyze intra-cluster distribution.
- Stacked bar charts to show relationships between customer segments and features like Profession, Graduated, and Spending_Score.

## Insights
- Two main customer segments were identified:
- Budget Customers: Generally younger with smaller family sizes and lower work experience.
Premium Customers: Tend to be older, with higher work experience, and exhibit higher spending scores.
Categorical features like Profession and Graduated status show distinct trends across segments.
# Technologies Used
Python (Pandas, NumPy, Matplotlib, Seaborn)
Scikit-learn (KMeans, PCA, LabelEncoder, RobustScaler, silhouette_score)

