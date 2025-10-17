
## 🧩 Customer Segmentation using K-Means Clustering

This project applies **K-Means Clustering** to the **Mall Customers Dataset** to group customers based on their **demographics and spending behavior**.
It helps retail businesses identify different customer segments for better marketing, personalization, and decision-making.

---

## 📊 Problem Statement

Retail businesses often deal with thousands of customers with varying purchasing behaviors.
Manually identifying these customer groups is inefficient and inaccurate.

**Goal:**
Use **machine learning (K-Means clustering)** to automatically group customers with similar characteristics such as:
- Gender
- Age
- Annual Income
- Spending Score

---

## 🎯 Objectives

- Analyze customer data to find natural clusters (segments).
- Identify **high-value**, **moderate**, and **low-value** customer groups.
- Visualize clusters in **2D and 3D** for clear interpretation.
- Provide actionable insights for marketing and business strategies.

---

## 🧰 Technologies & Tools Used

| Category | Tools |
|-----------|-------|
| Language | Python |
| Libraries | Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn |
| Environment | Google Colab |
| Algorithm | K-Means Clustering |

---

## 🧩 Dataset Information

**Dataset Name:** Mall_Customers.csv
**Columns:**
| Column | Description |
|---------|-------------|
| CustomerID | Unique customer ID |
| Gender | Male / Female |
| Age | Age of the customer |
| Annual Income (k$) | Annual income in thousands |
| Spending Score (1–100) | Score assigned based on customer spending behavior |

---

## ⚙️ Project Workflow

1. **Data Loading & Exploration**
   - Read dataset using Pandas
   - View summary statistics and structure

2. **Data Preprocessing**
   - Encode `Gender` (Male=1, Female=0)
   - Standardize numerical features for fair clustering

3. **Finding Optimal Clusters (Elbow Method)**
   - Tested `k = 1` to `10`
   - Selected `k = 5` based on the “elbow point”

4. **Model Training (K-Means)**
   - Applied K-Means with `n_clusters = 5`
   - Assigned each customer to a segment

5. **Visualization**
   - 2D plot: Income vs Spending Score
   - 3D plot: Age vs Income vs Spending Score

6. **Cluster Profiling**
   - Computed average Age, Income, and Spending Score per cluster
   - Interpreted segment behavior

---

## 📈 Results

- **5 clusters** were identified:
  1. 💸 **High Income, High Spending** – Premium customers
  2. 💰 **High Income, Low Spending** – Potential loyal customers
  3. 🛍️ **Low Income, High Spending** – Impulsive or budget spenders
  4. 👥 **Average Income, Moderate Spending** – Regular customers
  5. 💡 **Low Income, Low Spending** – Price-conscious group

- Achieved **clear visual separation** between customer groups.
- Generated insights useful for **targeted marketing** and **customer retention** strategies.

---

## 📊 Visualizations

- **Elbow Method Plot** – to find optimal number of clusters
- **2D Scatter Plot** – Income vs Spending Score
- **3D Cluster Plot** – Age, Income, Spending Score

---

## 💾 Output Files

- `Clustered_Customers.csv` → contains all customers with assigned cluster labels.

---

## 🚀 How to Run This Project

1. Open in **Google Colab**
   [Open in Colab ▶️](https://colab.research.google.com/github/yourusername/customer-segmentation-kmeans/blob/main/Customer_Segmentation_KMeans.ipynb)

2. Upload the dataset `Mall_Customers.csv`

3. Run each cell step by step (from data loading to visualization)

4. Download the clustered results file from the final step.

---

## 📚 Future Improvements

- Apply **Hierarchical Clustering** for comparison
- Use **Principal Component Analysis (PCA)** for dimensionality reduction
- Deploy model as a **Streamlit dashboard** for interactive segmentation

---

## 👩‍💻 Contributors

- **Your Name** – Data Analysis & Model Implementation
- (Add teammates’ names if this was a group project)

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).
