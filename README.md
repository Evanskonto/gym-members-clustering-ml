# Gym Members Clustering using Machine Learning

This project applies **KMeans** and **Hierarchical Clustering** to segment gym members based on their demographic, behavioural, and physiological metrics.  
It is based on a Kaggle dataset of 973 rows and was developed as part of my Data Analytics coursework.

The goal is to identify meaningful fitness personas that gyms can use to personalise training plans and improve member retention.

---

## 📌 Project Overview
- Dataset: *gym_members_exercise_tracking.csv* (Kaggle)
- Rows: 973
- Features include:
  - Age, BMI, Resting BPM, Max BPM
  - Calories Burned, Workout Frequency
  - Fat Percentage, Sleep Hours
  - VO₂ MAX, Body Temperature
- Applied clustering to detect the natural grouping of gym members.
- Main algorithms:
  - **KMeans Clustering**
  - **Agglomerative Hierarchical Clustering**

---

## 🧠 Techniques Used

### Preprocessing
- Missing value handling  
- Scaling using **StandardScaler**  
- Feature selection based on correlation  
- Outlier review  

### Clustering Models
- **KMeans (k = 3)** – chosen using:
  - Elbow Method  
  - Silhouette Score  
- **Hierarchical Clustering** – validated visually using a dendrogram

### Evaluation
- Silhouette score  
- Visual cluster separation  
- Comparison between algorithms  

---

## 📊 Key Results

### ✔ Optimal number of clusters: **3**
Representing:

#### **Cluster 0 — Beginners**
- Higher BMI  
- Low workout frequency  
- Fewer calories burned  

#### **Cluster 1 — Intermediate**
- Balanced metrics  
- Good workout routine  
- Normal heart rate profile  

#### **Cluster 2 — Advanced**
- Low fat %  
- High calorie expenditure  
- High workout consistency  

These profiles can help gyms create personalised programmes or targeted recommendations.

---

## 📷 Visualisations

All plots are available in the `results/` folder:

- `elbow_method.png`  
- `silhouette_score.png`  
- `kmeans_clusters.png`  
- `hierarchical_dendrogram.png`  
- `cluster_profiles.png`  

They showcase the workflow and separation between clusters.

---

## 📁 Repository Structure
