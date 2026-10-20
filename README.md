# Google Local Guides — User Segmentation & Predictive Analytics

### Data Analytics | Machine Learning | Power BI

An end-to-end data analytics project exploring user preferences across different travel and leisure attraction categories using Google Local Guides review ratings.

The project combines **Python-based data cleaning, exploratory data analysis, K-Means clustering, machine-learning classification, and interactive Power BI dashboards** to identify user behaviour patterns and visualize analytical results.

Developed as part of the **SWA2124 — Social and Web Analytics** coursework.

## Project Objectives

- Clean and preprocess Google review-rating data.
- Identify patterns in user preferences across attraction categories.
- Segment users based on their rating behaviour.
- Predict user segment membership using classification algorithms.
- Compare machine-learning model performance.
- Present findings through interactive Power BI dashboards.

## Dataset

**Dataset:** Google Local Guides Review Ratings

The dataset contains approximately **5,456 users** and their average ratings across **24 attraction categories**.

Categories include restaurants, beaches, hotels, museums, shopping malls, parks, cafes, art galleries, gyms, gardens, and other attractions.

Each user is represented by their rating preferences across these categories.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data processing and machine learning |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib & Seaborn | Exploratory data visualization |
| Scikit-learn | Clustering and classification |
| Google Colab | Python notebook development |
| Power BI | Interactive dashboards |

## Project Workflow

### 1. Data Cleaning and Preprocessing

The dataset was prepared for analysis using Python.

Key operations included:

- Examining data types and missing values.
- Identifying and removing structurally misaligned records.
- Removing unnecessary columns.
- Converting rating values to numeric types.
- Handling missing values using median imputation.
- Checking duplicate users and rating ranges.
- Investigating zero ratings and treating invalid zeros as missing values.
- Creating indicators for selected categories that were not rated.
- Exporting the cleaned dataset.

### 2. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to understand rating distributions and relationships between attraction categories.

Techniques included:

- Descriptive statistics.
- Correlation heatmaps.
- Rating distribution histograms.
- Skewness analysis.
- Identification of highly correlated attraction categories.

### 3. User Segmentation — K-Means Clustering

K-Means clustering was used to group users based on their rating preferences.

The modelling workflow included:

- Standardizing numerical features using StandardScaler.
- Applying Principal Component Analysis (PCA).
- Evaluating cluster counts using the Elbow Method and Silhouette Score.
- Implementing K-Means clustering.
- Visualizing clusters using a two-dimensional PCA projection.
- Comparing average attraction ratings across clusters.

The notebook uses **four clusters** as its configured segmentation setting.

### 4. Predictive Classification

Classification algorithms were applied to predict user segment membership from rating features.

Three models were included:

- Random Forest Classifier
- Logistic Regression
- Support Vector Machine (SVM)

Model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrices
- Stratified cross-validation

Feature importance analysis was also performed using Random Forest.

### 5. Power BI Dashboard

An interactive Power BI report was developed to visualize the analytical results.

**Page 1 — Overview**

Provides a general summary of the dataset, including:

- Total users
- Overall average rating
- Number of attraction categories
- Highest-rated category
- Average ratings by attraction category
- Rating distribution
- Cluster filtering

**Page 2 — Segments**

Explores the K-Means user segmentation results through:

- Cluster distribution donut chart
- Attraction-category rating comparisons
- Cluster profile matrix
- Interactive cluster slicer

**Page 3 — Models**

Presents predictive classification results through:

- Model comparison visualizations
- Performance metrics table
- Confusion matrix
- Model selection slicer

## Project Files

```text
Google-Local-Guides-Analytics/
│
├── SWA2124_fixed.pbix
├── SWA2124_data_cleaning_updated.ipynb
└── README.md
```

The Python notebook also generates CSV outputs for cleaned data, cluster assignments, cluster profiles, model comparisons, and confusion matrices.

## How to Run

### Python Notebook

1. Open Google Colab.
2. Upload `SWA2124_data_cleaning_updated.ipynb`.
3. Obtain the `google_review_ratings.csv` dataset.
4. Upload the dataset to Google Colab or Google Drive.
5. Update the dataset file path in the notebook.
6. Run the notebook cells in order.
7. Review the cleaning results, visualizations, clustering, and model evaluations.

### Power BI Dashboard

1. Install Power BI Desktop.
2. Download `SWA2124_fixed.pbix`.
3. Open the file in Power BI Desktop.
4. If prompted, update the data-source paths to the generated CSV files.
5. Refresh the dataset.
6. Explore the Overview, Segments, and Models pages.

**Note:** Power BI Desktop is required to interact with the `.pbix` report. GitHub stores the file but does not render an interactive Power BI dashboard.

## Skills Demonstrated

- Data cleaning and preprocessing
- Exploratory data analysis
- Feature engineering
- K-Means clustering
- Principal Component Analysis
- Predictive classification
- Machine-learning model evaluation
- Data visualization
- Power BI dashboard development
- Analytical reporting

## Future Improvements

- Experiment with alternative clustering algorithms.
- Optimize classification model hyperparameters.
- Add more detailed user-segment descriptions.
- Automate the data-cleaning and reporting pipeline.
- Deploy the dashboard through Power BI Service where permitted.

## Project Status

University data analytics and machine-learning project with a Python notebook and Power BI report.

## Developer

**Ania Ahmed**

Bachelor of Information Systems (Hons), Data Analytics

Sunway University, Malaysia

