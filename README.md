# 🏠 Large-Scale Geographic Consumer Clustering & High-Dimensional Visualizations

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-KMeans-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Folium](https://img.shields.io/badge/Folium-Interactive%20Maps-brightgreen)

---

## 📌 Project Overview

This project applies **Machine Learning (K-Means Clustering)** to analyze a real estate dataset and identify groups of properties with similar characteristics. The clustering process is based on geographical and housing features such as house age, MRT station distance, convenience stores, latitude, longitude, and house prices.

To better understand the clustering results, **Principal Component Analysis (PCA)** is used for dimensionality reduction, and **Folium** is used to create an interactive geographic visualization.

---

# 🎯 Problem Statement

Large real estate datasets contain multiple features, making it difficult to identify meaningful patterns manually. This project uses Machine Learning techniques to cluster similar properties and visualize the results on an interactive geographic map, making market segmentation easier to understand.

---

# 🎯 Objectives

- Load and preprocess the real estate dataset.
- Perform Exploratory Data Analysis (EDA).
- Select important features for clustering.
- Standardize the dataset using StandardScaler.
- Determine the optimal number of clusters using the Elbow Method.
- Apply the K-Means clustering algorithm.
- Reduce dimensions using PCA.
- Visualize property clusters using an interactive Folium map.
- Export the clustered dataset and interactive map.

---

# ⭐ Key Features

- 📊 Exploratory Data Analysis (EDA)
- 🤖 K-Means Clustering
- 📉 Elbow Method
- 📈 PCA Visualization
- 🌍 Interactive Geographic Map
- 📍 Cluster Visualization
- 💾 Export Clustered Dataset
- 🗺️ Interactive HTML Map

---

# 📂 Dataset

The project uses the **Real Estate Valuation Dataset**.

## Dataset Features

| Feature | Description |
|----------|-------------|
| X1 Transaction Date | Date of property transaction |
| X2 House Age | Age of the house |
| X3 Distance to MRT Station | Distance to the nearest MRT station |
| X4 Number of Convenience Stores | Number of nearby convenience stores |
| X5 Latitude | Latitude coordinate |
| X6 Longitude | Longitude coordinate |
| Y House Price of Unit Area | House price per unit area |

---

# 🛠 Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Folium

---

# 📚 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

from sklearn.preprocessing import StandardScaler
from sklearn.cluster import KMeans
from sklearn.decomposition import PCA

import folium
```

---

# 🔄 Machine Learning Workflow

## 1️⃣ Data Loading

- Loaded the dataset using Pandas.
- Displayed the first few records.

---

## 2️⃣ Data Exploration

- Displayed dataset information.
- Checked summary statistics.
- Verified missing values.

---

## 3️⃣ Feature Selection

Selected the following features:

- House Age
- Distance to MRT Station
- Number of Convenience Stores
- Latitude
- Longitude
- House Price

---

## 4️⃣ Data Scaling

Applied **StandardScaler** to normalize all selected features before clustering.

---

## 5️⃣ Elbow Method

Calculated WCSS values for different cluster numbers.

Generated the Elbow graph to determine the optimal number of clusters.

---

## 6️⃣ K-Means Clustering

Applied K-Means clustering to group similar properties.

Assigned cluster labels to every property.

---

## 7️⃣ PCA Visualization

Reduced six-dimensional data into two principal components.

Generated a scatter plot showing the clustered properties.

---

## 8️⃣ Interactive Geographic Visualization

Created an interactive Folium map using latitude and longitude.

Each property is displayed using a colored marker based on its assigned cluster.

Clicking on a marker displays:

- Cluster Number
- House Price
- House Age

---

# 🌍 Interactive Map

The project generates an interactive geographic visualization using **Folium**.

### Map Features

- 📍 Geographic property visualization
- 🎨 Different colors for each cluster
- 🔍 Zoom and Pan functionality
- 💬 Interactive pop-up information
- 🏠 House details displayed on click

### Interactive Map File

```
Real_Estate_Clusters.html
```

> **Note:** GitHub's notebook preview may not display interactive Folium maps because it does not consistently execute the JavaScript required by Folium.

### How to View the Interactive Map

1. Download **Real_Estate_Clusters.html** from the repository.
2. Open it using Chrome, Edge, Firefox, or any modern web browser.
3. Explore the clustered properties interactively.

---

# 🖼️ Map Preview



---

# 📊 Project Outputs

The project generates the following outputs:

- ✅ Elbow Method Graph
- ✅ PCA Cluster Visualization
- ✅ Clustered Dataset (`Real_Estate_Clustered.csv`)
- ✅ Interactive Map (`Real_Estate_Clusters.html`)

---

# 📁 Project Structure

```
Large-Scale-Geographic-Consumer-Clustering-High-Dimensional-Visualizations/
│
├── ML_TASK_3.ipynb
├── Real_Estate.csv
├── Real_Estate_Clustered.csv
├── Real_Estate_Clusters.html
├── README.md
└── map_preview.png   (Optional)
```

---

# 📈 Results

- Successfully clustered real estate properties using K-Means.
- Reduced high-dimensional data using PCA.
- Visualized clusters using scatter plots.
- Created an interactive geographic visualization using Folium.
- Exported clustered data for further analysis.

---

# 🚀 Future Enhancements

- Implement DBSCAN clustering.
- Compare with Hierarchical Clustering.
- Evaluate clusters using Silhouette Score.
- Develop a Streamlit dashboard.
- Add predictive analysis for house prices.

---

# ▶️ How to Run the Project

### Clone the Repository

```bash
git clone https://github.com/VasundhraVS/Large-Scale-Geographic-Consumer-Clustering-High-Dimensional-Visualizations.git
```

### Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn folium
```

### Run the Notebook

Open:

```
ML_TASK_3.ipynb
```

using **Google Colab** or **Jupyter Notebook** and run all cells sequentially.

---

# 📝 Note

- The notebook works correctly in **Google Colab** and **Jupyter Notebook**.
- GitHub may not display the interactive Folium map inside the notebook preview because of rendering limitations.
- The interactive version of the map is available in:

```
Real_Estate_Clusters.html
```

---

# 👩‍💻 Author

**Vasundhra VS**

Machine Learning | Python | Data Analytics | Data Visualization

---

⭐ If you found this project useful, consider giving it a star on GitHub!
