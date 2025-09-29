# Clothing Review Embedding Search

![Clothing Reviews](images/clothing.jpg)

Welcome to the world of e-commerce, where customer feedback is a goldmine of insights!  
This project analyzes the **Women's Clothing E-Commerce Reviews** dataset, focusing on the `Review Text` column filled with direct customer opinions.

Using **Python, OpenAI embeddings, ChromaDB, scikit-learn, NumPy, Pandas, Matplotlib, and t-SNE**, this project demonstrates how AI and ML can uncover themes, perform semantic searches, and visualize customer sentiments.  

The goal is to highlight how text embeddings and retrieval can improve **customer service, product offerings, and overall user experience**.

---

## ✨ Features

- **Semantic Search with Embeddings**: Uses OpenAI API to generate text embeddings of clothing reviews.
- **Vector Database**: Stores and queries embeddings with ChromaDB for efficient semantic search and retrieval.
- **Dimensionality Reduction**: Applies t-SNE (via scikit-learn) to cluster reviews and reveal patterns in sentiment and topics.
- **Visualisation**: Provides 2D plots of embeddings to illustrate clusters and semantic groupings.
- **Pythonic Best Practices**: Modular, reproducible workflow using Pandas, NumPy, and clear code structure.
- **Production Awareness**: Environment variables for security, scalable database integration, and reproducible results.

---

## 🛠️ Tech Stack

- **Language**: Python3 
- **AI/ML Services**: OpenAI API for embeddings
- **Vector Database**: ChromaDB
- **Data Processing**: NumPy, Pandas
- **Dimensionality Reduction**: scikit-learn (t-SNE)
- **Visualizations**: Matplotlib
- **Development Practices**: Environment variables for secrets, reproducible workflows

---

## 📊 The Data

**File:** `womens_clothing_e-commerce_reviews.csv`

| Column       | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| `Review Text`| Textual feedback provided by customers about their shopping experience and product quality. |

---

## ⚙️ Setup Instructions

### 1. Environment Variables
Before running the notebook, you must set your OpenAI API key:  
```bash
export OPENAI_API_KEY="your_api_key_here"
```
> Note: The dataset is provided in the notebook for demo purposes. For production use, connect to your own data source.

### 2. Clone the repository
```bash
git clone https://github.com/PL2134/clothing-review-embedding-search.git
cd clothing-review-embedding-search
```

### 3. Create a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### 4. Install dependencies
```bash
pip install -r requirements.txt
```

### 5. Set environment variables
Create a `.env` file in the project root with the following:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

(Your OpenAI key is required to generate embeddings.)

### 6. Run the notebook
Launch Jupyter or VSCode and open `clothing_review_embedding.ipynb` to run the workflow.

---

## 🚀 Future Improvements

- Dockerise workflow for containerised deployment  
- Deploy as a web service (Streamlit/Flask) with API endpoints  
- Integrate monitoring dashboards (Grafana/Prometheus) for runtime metrics  
- Experiment with additional vector DBs (e.g. FAISS, Pinecone)  
- Explore deployment on **GCP Vertex AI** or similar platforms  

---
