# 📄 Document Clustering & Query Reformulation

This project demonstrates **document clustering and query reformulation** using **K-Means** and **cosine similarity**. The goal is to determine relevant and irrelevant documents for a query and analyze how query reformulation affects retrieval performance.

---

## 🔍 Features
- **TF-IDF vectorization** to represent documents and queries.  
- **K-Means clustering (k=3)** to group documents based on semantic similarity.  
- **Cosine similarity** to evaluate query-document alignment.  
- **Rocchio-style query reformulation**:
  - Move query **closer to relevant cluster**  
  - Move query **closer to irrelevant cluster**  
  - Move query **further from relevant cluster**  
- Generates a **similarity comparison table** and a **one-page summary report**.

---

## 📊 Dataset
10 AI-related documents covering:
- Wearable devices & fitness  
- AI & NLP applications  
- Health monitoring & smart devices  

**Query used:**  
> "An application that uses AI to analyze fitness and health data from wearable devices."

---

## 🔑 Results
**Clusters identified:**  
- **Cluster 0 (Relevant):** D3, D4, D5, D7, D8, D9  
- **Cluster 1 (Irrelevant):** D2, D10  
- **Cluster 2 (Neutral):** D1, D6  

Reformulated queries demonstrated how moving the query vector affects similarity:
- Closer to relevant → similarity with D3, D5, D9 increases  
- Closer to irrelevant → similarity with D2, D10 increases slightly  
- Further from relevant → similarity with relevant documents drops

---

## ⚙️ Tech Stack
- Python  
- Scikit-learn (TF-IDF, KMeans, cosine similarity)  
- NumPy, Pandas  
- Google Colab / Jupyter Notebook  

---

## 📁 Output
- `similarity_results.csv` – document similarities before and after reformulation  
- `one_page_summary.txt` – concise analysis and interpretation  


- `similarity_results.csv` – document similarities before and after reformulation  
- `one_page_summary.txt` – concise analysis and interpretation  

