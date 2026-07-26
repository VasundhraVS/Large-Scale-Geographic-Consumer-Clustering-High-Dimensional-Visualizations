# Large-Scale Geographic Consumer Clustering & High-Dimensional Visualizations

## Project Overview

This project applies **Machine Learning (K-Means Clustering)** to analyze a real estate dataset and identify groups of properties with similar characteristics. The dataset includes features such as house age, distance to the nearest MRT station, number of convenience stores, geographical coordinates, and house prices.

The project also uses **Principal Component Analysis (PCA)** for dimensionality reduction and **Folium** to create an interactive geographic visualization of the clustered properties.

---

## Objectives

- Load and preprocess the real estate dataset.
- Perform exploratory data analysis.
- Select important features for clustering.
- Standardize the data using StandardScaler.
- Determine the optimal number of clusters using the Elbow Method.
- Apply the K-Means clustering algorithm.
- Reduce dimensions using PCA for visualization.
- Create an interactive map showing clustered properties using Folium.

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Folium

---

## Dataset

The project uses the **Real Estate Valuation Dataset**, which contains information about:

- House Age
- Distance to the nearest MRT Station
- Number of Convenience Stores
- Latitude
- Longitude
- House Price of Unit Area

---

## Machine Learning Workflow

### 1. Data Loading
- Imported the dataset using Pandas.

### 2. Data Exploration
- Displayed dataset information.
- Checked summary statistics.
- Verified missing values.

### 3. Feature Selection
Selected the following features:
- House Age
- Distance to MRT Station
- Number of Convenience Stores
- Latitude
- Longitude
- House Price

### 4. Data Scaling
Applied **StandardScaler** to normalize all features before clustering.

### 5. Elbow Method
Used the Elbow Method to determine the optimal number of clusters.

### 6. K-Means Clustering
Applied K-Means to group similar properties into clusters.

### 7. PCA Visualization
Reduced the dataset to two dimensions using PCA for visualization.

### 8. Interactive Map
Created an interactive Folium map displaying clustered properties based on their geographical locations.

---

## Project Outputs

- Clustered Dataset (CSV)
- Elbow Method Graph
- PCA Cluster Visualization
- Interactive Folium Map

---

## Project Structure

```
Large-Scale-Geographic-Consumer-Clustering-High-Dimensional-Visualizations/
│
├── ML_TASK_3.ipynb
├── Real_Estate.csv
├── Real_Estate_Clustered.csv
├── Real_Estate_Clusters.html
├── README.md
```

---

## Results

The K-Means algorithm successfully grouped similar properties into clusters based on geographical location and housing characteristics.

The PCA visualization clearly shows the separation between different property clusters.

The Folium map provides an interactive geographic visualization, allowing users to explore clustered properties on a map.

---

## Note

The interactive Folium map works correctly in **Google Colab** and **Jupyter Notebook**.

GitHub's notebook preview may not render interactive Folium maps because it does not consistently execute the JavaScript required by Folium.

To view the interactive map, open:

```
Real_Estate_Clusters.html
```

in any modern web browser.

---

## Future Improvements

- Apply DBSCAN and Hierarchical Clustering for comparison.
- Build an interactive dashboard using Streamlit.
- Add customer segmentation based on additional demographic features.
- Perform cluster evaluation using Silhouette Score and Davies-Bouldin Index.

---
