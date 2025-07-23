# 🤖 AI-Powered Resume Screening System  
**Team:** Capsule Corporation  

## 📌 Overview  
This project is an intelligent HR candidate screening system that evaluates resumes across multiple dimensions — fraud detection, professional network strength, experience, and skill synergy. The system outputs a dashboard that helps HR teams make data-driven and fair hiring decisions.

---

## 🔧 Components  

### 1. 🕵️ Fraud Detection System  
Calculates a **Risk Score** using:
- **Text Similarity Score** (50%): Measures similarity between resumes and recommendation letters using TF-IDF and Cosine Similarity.
- **Vague Words Score** (30%): Flags generic language in recommendation letters.
- **Reciprocal Detection Score** (20%): Detects mutual or biased endorsements.

Outlier detection via boxplots flags suspicious candidates.

### 2. 🌐 Network Connection Analysis  
Calculates a **Network Connection Score** using:
- **Centrality Measures**: Betweenness, Closeness, In-Degree, Out-Degree.
- **Community Score**: Based on Louvain community detection.

Final Score = 0.8 × Centrality Score + 0.2 × Community Score

### 3. 📊 HR Decision Dashboard  
Ranks candidates using:
- Risk Score (30%)
- Network Score (30%)
- Experience (20%)
- Skill Synergy (20%)

Provides side-by-side comparison and highlights red flags visually.

---

## 🤝 Google Gemini + RAG for Resume Parsing  
- Resumes parsed using `pdfplumber`.
- Structured data extracted via **Google Gemini** using a Retrieval-Augmented Generation (RAG) pipeline.
- Output validated and cleaned to ensure consistency across formats.

---

## ⚖️ Fairness & Ethics  
- Applied bias detection tools to reduce gender/racial NLP bias.
- Candidates compared within peer communities.
- No demographic filtering used.

---

## 🚀 Scalability  
- Parallelized resume processing.
- Optimized for large networks using scalable community detection algorithms.

---

## 🧰 Tech Stack  
- Python (pandas, scikit-learn, networkx, pdfplumber)  
- Google Gemini (LLM)  
- Louvain Algorithm  
- TF-IDF, Cosine Similarity  
- Streamlit / Dash (for UI)

---

## ✅ Key Outcomes  
- Risk scores successfully flagged weak or suspicious profiles.  
- Network scores revealed candidate influence and connectivity.  
- Skill synergy analysis helped validate listed vs practical skills.  
- Dashboard enabled transparent, fair, and data-driven decisions.

---

## 📬 Contact  
For questions or collaboration, reach out to the Capsule Corporation team.

