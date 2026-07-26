# Large-Scale Geographic Consumer Clustering & High-Dimensional Visualizations

## Project Overview

This project applies **Machine Learning (K-Means Clustering)** to analyze a real estate dataset and identify groups of properties with similar characteristics. The dataset includes information such as house age, distance to the nearest MRT station, number of convenience stores, geographical coordinates, and house prices.

The project also uses **Principal Component Analysis (PCA)** to reduce high-dimensional data into two dimensions for visualization and **Folium** to create an interactive geographic map of clustered properties.

---

# Problem Statement

Large real estate datasets contain multiple features that make it difficult to identify meaningful patterns manually. This project aims to cluster similar properties based on their geographical and housing characteristics, helping users understand market segments through machine learning and interactive visualizations.

---

# Objectives

- Load and preprocess the real estate dataset.
- Perform exploratory data analysis.
- Select important features for clustering.
- Standardize numerical features.
- Determine the optimal number of clusters using the Elbow Method.
- Apply the K-Means clustering algorithm.
- Visualize clusters using PCA.
- Display clustered properties on an interactive Folium map.
- Save the clustered dataset and interactive map.

---

# Dataset

The project uses the **Real Estate Valuation Dataset**.

### Features

| Feature | Description |
|---------|-------------|
| X1 Transaction Date | Date of property transaction |
| X2 House Age | Age of the house |
| X3 Distance to MRT Station | Distance to the nearest MRT station |
| X4 Number of Convenience Stores | Number of nearby convenience stores |
| X5 Latitude | Latitude coordinate |
| X6 Longitude | Longitude coordinate |
| Y House Price of Unit Area | House price per unit area |

---

# Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Folium

---

# Libraries Used

```python
pandas
numpy
matplotlib
sklearn
folium
```

---

# Machine Learning Workflow

## 1. Data Loading

- Imported the dataset using Pandas.
- Displayed the first few records.

## 2. Data Exploration

- Checked dataset information.
- Displayed summary statistics.
- Verified missing values.

## 3. Feature Selection

Selected the following features:

- House Age
- Distance to MRT Station
- Number of Convenience Stores
- Latitude
- Longitude
- House Price

## 4. Data Scaling

Applied **StandardScaler** to normalize the selected features before clustering.

## 5. Elbow Method

Calculated WCSS values for different cluster numbers and plotted the Elbow graph to determine the optimal number of clusters.

## 6. K-Means Clustering

Applied K-Means clustering to group similar properties.

## 7. Cluster Assignment

Assigned cluster labels to each property and stored them in a new column.

## 8. PCA Visualization

Reduced six-dimensional data into two principal components for visualization.

Generated a scatter plot showing different property clusters.

## 9. Interactive Geographic Visualization

Created an interactive Folium map using the latitude and longitude coordinates.

Each property is displayed as a colored marker based on its assigned cluster.

Clicking on a marker displays:

- Cluster Number
- House Price
- House Age

---

# Interactive Map

The project generates an interactive HTML map using Folium.

### Features

- Interactive zoom
- Colored cluster markers
- Property information popup
- Geographic visualization
- Easy exploration of clustered properties

The generated map is saved as:

```
Real_Estate_Clusters.html
```

---

# Output Files

The project generates the following outputs:

- Elbow Method Graph
- PCA Cluster Visualization
- Clustered Dataset (`Real_Estate_Clustered.csv`)
- Interactive Folium Map (`Real_Estate_Clusters.html`)

---

# Project Structure

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

# Results

- Successfully identified different groups of properties using K-Means clustering.
- Reduced high-dimensional data using PCA for easy visualization.
- Generated an interactive geographic map showing clustered properties.
- Saved the clustered dataset for further analysis.

---

# Future Enhancements

- Compare with DBSCAN clustering.
- Apply Hierarchical Clustering.
- Build a Streamlit dashboard.
- Add Silhouette Score evaluation.
- Integrate additional housing features.

---

# How to Run the Project

1. Clone the repository.

```
git clone https://github.com/VasundhraVS/Large-Scale-Geographic-Consumer-Clustering-High-Dimensional-Visualizations.git
```

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Install the required libraries.

```
pip install pandas numpy matplotlib scikit-learn folium
```

4. Run all cells sequentially.

5. View the generated outputs.

---

# Note

The interactive Folium map displays correctly in **Google Colab** and **Jupyter Notebook**.

GitHub's notebook preview may not display the interactive map because it does not consistently execute the JavaScript required by Folium.

To view the interactive map, open:

```
Real_Estate_Clusters.html
```

in any modern web browser.

---

# Author

**Vasundhra VS**

Machine Learning | Python | Data Analytics | Data Visualization
