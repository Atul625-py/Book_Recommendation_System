# 📚 Book Recommendation System using STAMP

## 🧠 Overview
This project is developed as part of the **Intelligent Computing Project**.  
It implements a **Book Recommendation System** using the **STAMP (Short-Term Attention/Memory Priority)** model.  
The system intelligently recommends books based on user interaction sequences and preferences derived from the Kaggle dataset.

## 🚀 Features
- Personalized book recommendations based on user history.
- Implementation of **STAMP** model for sequence-based recommendation.
- Data preprocessing and feature extraction from Kaggle dataset.
- Integration-ready backend for recommendation API.
- Interactive frontend for exploring book suggestions.

## 🗂️ Tech Stack
- **Machine Learning:** STAMP model (TensorFlow / PyTorch)
- **Backend:** Django / FastAPI (for API serving)
- **Frontend:** React.js
- **Database:** SQLite / PostgreSQL
- **Dataset Source:** Kaggle Book Recommendation Dataset

## 👨‍💻 Team Members

| Role | Name | Roll Number | GitHub ID |
|------|------|--------------|-----------|
| ⭐ **Team Leader & ML Analyst & Backend Developer** | **Atul Kumar Pandey** | 23074006 | [Atul625-py](https://github.com/Atul625-py) |
| 🤝 **Frontend Developer** | **Chukka Chamantej** | 23074028 | [Chukkachaman](https://github.com/Chukkachaman) |
| 🎨 **Frontend Developer** | **Purushottam Lal** | 23075061 | [purushottam62](https://github.com/purushottam62) |

## 📈 Model Summary (STAMP)

**STAMP (Short-Term Attention/Memory Priority)** is a powerful neural architecture designed for **session-based recommendation systems**, particularly suited for modeling **short-term user behavior** while retaining essential aspects of their **long-term preferences**.

Unlike traditional recommendation models that rely solely on user history or item embeddings, STAMP dynamically captures the **temporal sequence of user interactions** within a session. It gives higher weight (attention) to the most relevant recent actions while still considering the user’s overall session context.

### 🧠 Key Components
- **Short-Term Attention Layer:**  
  Focuses on the most recent interactions in a session, identifying which past items are most relevant to the current prediction.  
- **Long-Term Memory Layer:**  
  Retains an aggregated representation of the user’s general preferences derived from previous sessions.  
- **Context Fusion Mechanism:**  
  Combines outputs from short-term attention and long-term memory to produce a context-aware user representation.  
- **Prediction Layer:**  
  Uses the fused representation to predict the next likely item (book) the user will interact with.

### ⚙️ Model Highlights
- Learns **both immediate and habitual behaviors**, improving recommendation quality for users with diverse interests.  
- Employs **attention mechanisms** for adaptive context weighting, enhancing interpretability.  
- Ideal for **cold-start or anonymous users** where explicit long-term profiles are unavailable (since it works on session data).  
- Efficiently handles **variable-length interaction sequences** and **noisy session data**.

### 🧩 Why STAMP for Books?
In a book recommendation context, user interests often vary between genres, authors, or moods within a single session.  
STAMP’s attention mechanism helps capture these subtle, evolving preferences — recommending the next book that best matches the **user’s immediate curiosity** while respecting their **overall taste**.
#
---

### 🎥 Find Presentation Here
[View on Canva](https://www.canva.com/design/DAG2anvGKac/2TJaV0EQOJblUQ5jcyiYZg/edit?utm_content=DAG2anvGKac&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

---


## 🧩 Folder Structure
```
BookRecommendationSystem/
│
├── data/                # Kaggle dataset files
├── model/               # STAMP model training scripts
├── backend/             # API & server logic
├── frontend/            # React frontend code
├── notebooks/           # Jupyter experiments and analysis
└── README.md
```
## ⚙️ Setup Instructions
1. Clone this repository:
   ```bash
   git clone https://github.com/Atul625-py/Book_Recommendation_System.git
   cd Book_Recommendation_System
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Train the model:
   ```bash
   python model/train_model.py
   ```

4. Setup and run the backend:
   ```bash
   cd backend
   python manage.py import_clean_data
   python manage.py makemigrations
   python manage.py migrate
   python manage.py runserver
   ```

5. In another terminal, start the frontend:
   ```bash
   cd frontend
   npm install
   npm run dev
   ```
   
---

## 📊 Dataset Source
[Kaggle - Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset)

## 🧩 Future Scope
- Add hybrid recommendation (content + collaborative).
- Include multilingual support for book titles.
- Deploy with Docker and integrate with cloud storage.
- Add user authentication and dynamic profiling.

---

### 🧑‍🏫 Project for Intelligent Computing Course
**IIT (BHU) Varanasi**
