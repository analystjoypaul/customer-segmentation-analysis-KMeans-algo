![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Libraries](https://img.shields.io/badge/Libraries-pandas%2C%20seaborn%2C%20sklearn-orange)
# Customer Segmentation using K-Means Clustering

## 🎯 Objective
- Segment mall customers into distinct groups based on their **purchasing behavior** and **demographic attributes**.
- Help businesses create **targeted marketing campaigns**.
- Enable **personalized customer experiences**.

## 📂 Dataset
- **File:** `Mall_Customers.csv`
- **Description:** Contains customer details:
  - Gender
  - Age
  - Annual Income (k$)
  - Spending Score (1–100)

## 🛠️ Steps Followed
1. **Import necessary libraries** and load the dataset.
2. **Explore and preprocess** the data.
3. Apply **K-Means clustering** to group customers.
4. **Visualize clusters** and interpret the results.

---
## The workflow is divided into three main sections:


## 1️⃣ Exploratory Data Analysis (EDA)

### **Age Distribution**
- Most customers are between **20–40 years old**.
- Customers aged **50+** are fewer, indicating a younger demographic skew.

### **Annual Income (in $1000s)**
- Income is concentrated between **$40k and $80k**.
- A small group earns above **$100k**, representing a limited high-income segment.

### **Spending Score (1–100)**
- Spending scores are spread across the range, with notable peaks between **40–60**, showing a large cluster of average spenders.
- Very low and very high spenders are less common.

![Customer Distribution](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Feature%20Distributions.png) 

---

### **Customer Age Group Analysis**
- **26–35 years**: Largest group (~60 customers), dominant demographic.
- **18–25 years**: ~34 customers, a significant young adult segment.
- **36–55 years**: ~30–34 customers, balanced middle-aged presence.
- **55+ years**: ~29 customers, smallest segment.

![Customer Distribution](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Age%20Group%20Distribution.png)

---

### **Spending Score Group Analysis**
- **41–60 range**: Largest group (~75 customers), average spenders.
- **1–20 range**: ~36 customers, very low spenders.
- **21–40 range**: Lowest (~27 customers), below-average spenders.
- **61–100**: ~30–32 customers, fewer high spenders.

![Customer Distribution](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Customer%20Count%20by%20Spending%20Score.png)

---

### **Annual Income vs Spending Score**
- No strong correlation between income and spending.
- Most customers fall in **$40k–$70k income** and **40–60 spending score**.
- Both genders have similar spending behavior.

![Annual Income vs Spending Score](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Annual%20Income%20vs%20Spending%20Score.png)

---

## 2️⃣ Elbow Method – Optimal Cluster Selection

The Elbow Method is used to determine the **optimal number of clusters (K)**:

- **WCSS** decreases as the number of clusters increases.
- The curve **bends at K = 5**.
- **Optimal number of clusters: 5**

![Elbow Method](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Elbow%20Method.png)

---
## 3️⃣ Customer Segmentation using K-Means Clustering

This plot shows how customers are grouped into 5 clusters based on their **Annual Income** and **Spending Score**.

![Customer Clusters](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Clustere%20of%20customer.png)

### 🔍 Key Observations:

- The plot shows **5 distinct customer groups**, identified using the K-Means algorithm.
- Each color represents a different cluster, and the black "X" marks show the **cluster centers**.
- The clusters help identify customer types such as:
  - 🟥 High spending, low income
  - 🟦 High income, high spending
  - 🟪 Average income, average spending
  - 🟧 Low income, low spending
  - 🟩 High income, low spending
    
## 🔗 Project Link
[Customer Segmentation using K-Means – Jupyter Notebook](https://github.com/BijoyBytes/customer-segmentation-using-k-means/blob/main/Customer%20Segmentation%20using%20K-Means%20Clustering.ipynb)

---

## 📌 Next Steps

- Use clustering results to build **targeted marketing strategies**.
- Potential extension: Deploy as a web app using **Streamlit**.

## 👤 Author
**Bijoy Paul**  
[GitHub](https://github.com/BijoyBytes) | [LinkedIn](https://www.linkedin.com/in/bijoybytes/)

## ⚙️ Requirements

```bash
pip install pandas matplotlib seaborn scikit-learn

