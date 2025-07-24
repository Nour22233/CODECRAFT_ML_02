🏷️ Task 02 – Customer Segmentation using K-Means
💻 Description
In this project, we implemented a K-Means Clustering algorithm to group retail store customers based on their purchase history. This enables the business to identify distinct customer segments and design targeted marketing strategies.

📂 Dataset
Name: Mall Customers Dataset

Source: Customer Segmentation Dataset on Kaggle

Features Used:

Annual Income (k$): Customer's yearly income.

Spending Score (1-100): Score assigned by the mall based on customer spending behavior.

Age and Gender were also explored for visualization and insights.

⚙️ Main Steps
Data Loading & Exploration

Loaded dataset with 200 rows and 5 columns.

Checked null values (0 missing) and duplicates (0 duplicated rows).

Visualized:

Age distribution (most customers aged between 20-40 years).

Spending Score distribution.

Pairplot to see relationships.

Scatter plots of Annual Income vs Spending Score.

Data Preprocessing

Encoded Gender to numeric (Male=0, Female=1).

Standardized numerical features using StandardScaler to improve clustering performance.

K-Means Clustering

Used Elbow Method to determine optimal k (found k=3 suitable).

Trained K-Means model with k=3 clusters.

Visualized clusters with centroids for clear segmentation.

Additional Clustering Techniques

DBSCAN Clustering:

Estimated number of clusters: 1.

Number of noise points: 199 (indicating DBSCAN did not fit this data well with current parameters).

Hierarchical Clustering:

Applied single, complete, average, and ward linkage methods.

Generated dendrograms for hierarchical analysis.

Evaluation Metrics

Silhouette Score: 0.4486

Calinski-Harabasz Index: 365.798

Davies-Bouldin Score: 0.884

📈 Results
Metric	Value
Silhouette Score	0.4486
Calinski-Harabasz	365.798
Davies-Bouldin Score	0.884

✅ Interpretation:

Clusters are reasonably separated (Silhouette > 0.4).

Calinski-Harabasz score indicates compact, well-defined clusters.

Low Davies-Bouldin score indicates good clustering quality.

📚 Libraries Used
pandas

numpy

matplotlib

seaborn

sklearn

StandardScaler

KMeans

DBSCAN

NearestNeighbors

metrics (silhouette_score, calinski_harabasz_score, davies_bouldin_score)

scipy.cluster.hierarchy



🔹 Task by: Nour Hesham
🔹 Internship: Machine Learning – Code Craft