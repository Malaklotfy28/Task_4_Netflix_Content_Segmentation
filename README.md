# Netflix Content Segmentation

## Project Overview

This project focuses on applying Unsupervised Machine Learning techniques to group Netflix titles into clusters based on their content characteristics.

It is **Task 4: Netflix Content Segmentation**, completed as part of the Machine Learning Internship at Auspify Technologies.

The project uses the K-Means clustering algorithm to discover patterns and similarities among Netflix movies and TV shows without requiring predefined target labels.

## Objective

The main objective is to group Netflix titles into meaningful clusters based on features such as content type, release year, duration, country, and genres.

The project also visualizes the resulting clusters and analyzes their characteristics to better understand the structure of the dataset.

## Dataset

The project uses a Netflix dataset stored in `Dataset.csv`.

The dataset includes the following columns:

- `show_id`: Unique identifier for each title.
- `type`: Whether the title is a Movie or TV Show.
- `title`: Title name.
- `director`: Director of the title.
- `country`: Country associated with the title.
- `date_added`: Date the title was added to Netflix.
- `release_year`: Original release year.
- `rating`: Audience rating category.
- `duration`: Movie duration or number of seasons.
- `listed_in`: Genres and categories.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Workflow

### 1. Data Loading and Exploration

- Loaded the Netflix dataset using Pandas.
- Examined dataset dimensions and column names.
- Checked data types and missing values.
- Identified duplicate records.

### 2. Data Preprocessing

- Handled missing values in the selected features.
- Extracted numerical values from the duration column.
- Prepared numerical and categorical features for clustering.

### 3. Feature Engineering

Selected features for clustering:

- Content type
- Release year
- Duration
- Genre and category information
- Country

Applied one-hot encoding to transform categorical features into numerical representations.

### 4. Feature Scaling

Standardized the feature matrix using NumPy to reduce the influence of differences in numerical scales.

### 5. K-Means Clustering

Implemented the K-Means clustering algorithm using NumPy.

The algorithm assigns each title to a cluster based on its distance from the cluster centers and updates the centers iteratively.

The initial experiment uses five clusters (`k = 5`).

### 6. Cluster Visualization

Visualized the number of titles assigned to each cluster.

Applied Principal Component Analysis (PCA) using NumPy to reduce the feature space to two dimensions for visualization.

### 7. Cluster Analysis

Analyzed the resulting clusters by examining:

- Content type distribution
- Average release year
- Most frequent genres and categories

These analyses help identify patterns and differences between groups.

### 8. Exporting Results

Saved the processed dataset, including cluster assignments, to `Netflix_Content_Segmentation_Results.csv`.

## Results

The project produces five initial content clusters.

The clusters are visualized using a two-dimensional PCA scatter plot, and their characteristics are explored through summary tables.

The interpretation of each cluster should be based on the actual results obtained when running the notebook.

## Project Structure

```text
Task_4_Netflix_Content_Segmentation/
│
├── Task_4_Netflix_Content_Segmentation.ipynb
├── Dataset.csv
├── Netflix_Content_Segmentation_Results.csv
├── README.md
└── screenshots/
    ├── cluster_distribution.png
    └── cluster_visualization.png
```

## How to Run the Project

1. Clone or download the project repository.
2. Ensure Python is installed.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

4. Place `Dataset.csv` in the project directory.
5. Open the notebook using Jupyter Notebook or Visual Studio Code.
6. Run the notebook cells in order.
7. Review the cluster visualizations and analysis.
8. Check the generated `Netflix_Content_Segmentation_Results.csv` file.

## Skills Demonstrated

- Data exploration and preprocessing
- Feature engineering
- One-hot encoding
- Feature scaling
- Unsupervised Machine Learning
- K-Means clustering
- Principal Component Analysis (PCA)
- Cluster visualization and interpretation
- Python and NumPy

## Internship Information

**Program:** Machine Learning Internship

**Organization:** Auspify Technologies

**Task:** Task 4, Netflix Content Segmentation

This project provided practical experience in discovering patterns in data, implementing clustering algorithms, and visualizing the results of an Unsupervised Machine Learning workflow.
