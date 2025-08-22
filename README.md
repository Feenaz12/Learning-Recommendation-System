# 🎓 Learning Recommendation System

Recommending the right courses to students helps them improve skills, explore new areas, and achieve their career goals. This project analyzes student profiles and course data to provide personalized course recommendations using machine learning techniques.

---

## 🚀 Features

- Preprocess student and course data using **TF-IDF vectorization**  
- Recommend **top N courses** based on student profile (skills + interests)   
- Save and load **pretrained models & matrices** for fast recommendations  
- Display student info alongside recommended courses  

---

## 📊 Dataset

Two datasets are used:

| Dataset | Description |
|---------|-------------|
| `students.csv` | Student details: ID, name, background, skills, interests |
| `courses.csv` | Course details: ID, name, category, difficulty |

> **Tip:** Sample datasets for 1000 students and ~50 courses are provided. Replace with your own datasets for larger experiments.

---

## ⚡ Preprocessing

- **Profile Text:** Combine student skills + interests into one text field  
- **Vectorization:** TF-IDF vectorization for student profiles and course descriptions  
- **Similarity Computation:** Cosine similarity between student profiles and courses  
- **Saved Models:** Vectorizers and matrices stored as `.pkl` files for reuse  

---

## 🛠 Recommendation Logic

- Compute **cosine similarity** between student vector and all course vectors  
- Sort and select **top N courses** for recommendation  
- Display student details (name, background, skills, interests) along with recommended courses  

---

## 🔧 Tech Stack

- **Python** – Core programming language  
- **Pandas & NumPy** – Data manipulation and analysis  
- **Scikit-learn** – TF-IDF vectorization, cosine similarity, and ML utilities  
- **Joblib** – Save/load models and matrices  


```bash
python src/preprocess.py
