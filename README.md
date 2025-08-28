# 🎬 Netflix Movie Recommendation System (Correlation-Based)

This project demonstrates how to build a **movie/TV show recommender system** using **Item–Item Collaborative Filtering** with **correlation analysis**.  

It mimics how Netflix recommends shows such as *“Because you watched Dexter, you may enjoy Dahmer”* by analyzing user watch history and finding similarities between shows.

---

## 📂 Project Files
- **`Netflix Movie Recommendation Using Correlation.xlsx`**  
  - Raw dataset containing:
    - Subscriber IDs  
    - Show names  
    - Episodes watched  
    - Episode length (minutes)  
    - Total minutes watched  
  - Includes pivot tables, descriptive statistics, and an Excel-based correlation matrix.  

- **`netflix-movie-recommendation-model.ipynb`**  
  - Python Jupyter Notebook with an end-to-end implementation:
    - Data cleaning & preprocessing  
    - User–Item matrix creation  
    - Item–Item correlation matrix (Pearson)  
    - Recommendation functions:
      - `recommend_similar(show, ...)` → Global recommendations (“Because you liked X…”)  

---

## 🔑 Motivation
Recommendation systems power platforms like **Netflix, Spotify, and Amazon** by personalizing content for each user.  

This project was created to:
- Understand how collaborative filtering works in practice  
- Transform raw viewing history into actionable recommendations  
- Build a **Python implementation** of an Excel-based prototype  

---

## 📊 Key Concepts
- **Collaborative Filtering (Item–Item):**  
  Suggests items based on their similarity to other items the user has already consumed.  

- **Correlation Matrix (Pearson):**  
  Measures how strongly two shows are related based on audience overlap.  
  - +1 → strongly similar  
  - 0 → no relation  
  - –1 → inversely related  

- **Recommendation Types:**  
  - *Global* (show-to-show similarity)  

---

## 🚀 How to Run
1. Clone or download this repo.  
2. Open the notebook:  
   ```bash
   jupyter notebook netflix-movie-recommendation-model.ipynb
   ```
   
3. Install dependencies (if not already):
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
   ```
4. Run all cells to:

Load the Excel dataset

Build the correlation matrix

Visualize show-to-show similarities

Generate recommendations

---

## 🖼 Visualizations

Correlation Heatmap → relationships between shows

Bar Charts → top recommended shows per series

Series Recommendations → personalised top-k lists

---

## ✅ Learning Outcomes

Through this project, I learned to:

* Transform raw logs into a User–Item matrix

* Apply item–item collaborative filtering using correlation

* Build both global and personalized recommenders

* Visualise and interpret similarity scores in a business-friendly way

* Package a workflow from Excel prototype → Jupyter Notebook

---

## 📌 Future Improvements

* Add cosine similarity to handle sparse data better

* Experiment with user–user collaborative filtering

* Deploy as a simple web app (Streamlit/Flask) for interactive recommendations
  
