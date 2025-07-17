# Career-Nav-AI 🚀

**Career-Nav-AI** is an AI-powered job recommendation system that semantically matches user queries to the most relevant career roles using transformer-based embeddings and vector similarity search.

### 🔗 Live Demo  
*Coming Soon on Streamlit Cloud or Hugging Face Spaces*

---

## 🧠 How It Works

1. **Input:** The user enters a career interest or query (e.g., "creative design", "data science", etc.).
2. **Embedding:** The query is embedded using Hugging Face's `all-MiniLM-L6-v2` model.
3. **Similarity Search:** The system calculates cosine similarity with job role embeddings from a dataset.
4. **Output:** Returns the top 5 most relevant job titles along with metadata like:
   - Salary range
   - Required education level
   - Prestige rating
   - Description of duties

---

## 🔧 Tech Stack

| Layer         | Tools Used                                                  |
|---------------|-------------------------------------------------------------|
| Frontend      | Streamlit                                                   |
| NLP Model     | Hugging Face Transformers: `all-MiniLM-L6-v2`               |
| Embedding     | SentenceTransformers (`sentence-transformers`)              |
| Similarity    | Scikit-learn: `cosine_similarity`                           |
| Backend       | Python                                                      |
| Data Handling | Pandas + CSV datasets (`Duties.csv`, `Education.csv`, etc.)|

---

## 📂 Dataset Files

- `Duties.csv` – Job titles and responsibilities
- `Education.csv` – Required education levels per job
- `Salary.csv` – Income expectations
- `Prestige.csv` – Social prestige metrics
- `Geography.csv` – Location-based metadata (optional)

---

 



---

## 💬 Feedback Collection

Users can submit feedback on job matches via a simple text input, allowing for potential personalization and future fine-tuning.

---

## 🚀 Future Enhancements

- Integrate a **vector database** like FAISS or Pinecone for scalable similarity search.
- Add **real-time feedback loop** and personalization.
- Connect to a **live job API** (e.g., LinkedIn or Indeed).
- Deploy on **Streamlit Cloud** or Hugging Face Spaces.

---

## 🛠️ Installation

```bash
git clone https://github.com/milanrajani/career-nav-ai.git
cd career-nav-ai
pip install -r requirements.txt
streamlit run app.py
