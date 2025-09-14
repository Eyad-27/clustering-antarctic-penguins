# 🐧 Clustering Antarctic Penguin Species

![Penguin Illustration](https://imgur.com/orZWHly.png)  
*Source: [Allison Horst](https://github.com/allisonhorst/penguins)*

Researchers have collected data on Antarctic penguins but have not recorded their species.  
In this project, I applied **unsupervised machine learning (clustering)** to group penguins into clusters that reflect potential species (Adelie, Chinstrap, Gentoo) based on body measurements.

---

## 📌 Guiding Question  
- Can we use clustering techniques to identify natural groupings of penguins that may correspond to different species?  

---

## 📂 The Data

**File:** `penguins.csv`

| Column              | Description                |
|----------------------|----------------------------|
| `culmen_length_mm`  | Culmen (bill) length (mm) |
| `culmen_depth_mm`   | Culmen (bill) depth (mm)  |
| `flipper_length_mm` | Flipper length (mm)       |
| `body_mass_g`       | Body mass (g)             |
| `sex`               | Penguin sex               |

Dataset provided by **Dr. Kristen Gorman** and the **Palmer Station, Antarctica LTER** (Long Term Ecological Research Network).  

---

## 🛠️ Project Steps  

### 1. Data Preprocessing  
- Loaded `penguins.csv` and explored numerical & categorical features.  
- Created dummy variables for categorical features (`sex`) and dropped originals.  
- Standardized numerical values for clustering.  

### 2. Determining the Optimal Number of Clusters  
- Used the **Elbow method** to identify the best k for k-means clustering.  
- Selected an appropriate number of clusters (aligned with expected ~3 penguin species).  

### 3. Running K-Means Clustering  
- Applied **k-means algorithm** from scikit-learn.  
- Visualized clusters to confirm separation.  

### 4. Creating Cluster Statistics  
- Generated a final DataFrame (`stat_penguins`) with one row per cluster.  
- Calculated **mean values** of numeric features per cluster to describe species groups.  

---

## ✅ Key Deliverables  
- Preprocessed dataset with categorical encoding and scaling.  
- Identified optimal **k value** for clustering.  
- Performed k-means clustering on penguin measurements.  
- Created statistical summary DataFrame (`stat_penguins`) describing each cluster.  
- Produced cluster insights reflecting distinct penguin species traits.  

---

## 🧰 Skills Used  
- Python (`pandas`, `numpy`, `scikit-learn`)  
- Data preprocessing & feature engineering  
- Unsupervised learning (k-means clustering)  
- Elbow method for model selection  
- Cluster interpretation & statistical profiling  
