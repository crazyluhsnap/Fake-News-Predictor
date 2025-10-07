# 📰 Fake News Predictor

## 📘 Overview
This project is a **Machine Learning model** that predicts whether a given news article is **real or fake**.  
It uses **Natural Language Processing (NLP)** techniques and a **TF-IDF Vectorizer** to convert textual data into numerical form, followed by a **Logistic Regression classifier** to perform binary classification.

---

## ⚙️ Features
- Combines two datasets: **real news** and **fake news**
- Labels data as:  
  - `1` → Real News 🟢  
  - `0` → Fake News 🔴
- Text preprocessing and cleaning
- Uses **TF-IDF Vectorization** to extract important textual features
- Trains a **Logistic Regression** model for accurate predictions
- Evaluates model performance using **accuracy score**

---

## 🧠 Technologies Used
- **Python 3**
- **Pandas** — for data handling
- **NumPy** — for numerical operations
- **Scikit-learn** — for model building and evaluation
- **Matplotlib / Seaborn** — for visualization

---

## 📂 Dataset
The dataset includes two CSV files:
- `Fake.csv` — contains fake news articles
- `True.csv` — contains real news articles

Both datasets are merged, and a new column `label` is added:
```python
fake_news['label'] = 0
true_news['label'] = 1
news_dataset = pd.concat([fake_news, true_news], axis=0)
```

---

## 🔍 Model Workflow
1. **Data Preprocessing**
   - Remove missing values
   - Clean and normalize text
   - Combine fake and real datasets

2. **Text Vectorization**
   - Convert text into numerical form using **TF-IDF Vectorizer**

3. **Model Training**
   - Use **Logistic Regression** for binary classification
   - Split data into training and testing sets

4. **Evaluation**
   - Compute model accuracy
   - Display confusion matrix (optional)

---

## 📊 Example Output
```
Accuracy score: 0.98
The news is Real ✅
```

---

## 🚀 How to Run
1. Clone the repository
```bash
git clone https://github.com/<your-username>/Fake-News-Predictor.git
cd Fake-News-Predictor
```
2. Install dependencies
```bash
pip install -r requirements.txt
```
3. Run the notebook
```bash
jupyter notebook Fake_News_Predictor.ipynb
```

---

## 🧩 Future Improvements
- Use **LSTM / BERT** for deeper NLP understanding
- Add a **web interface** using Flask or Streamlit
- Include **real-time news validation** from APIs

---

## 👨‍💻 Author
**Panshul Gupta**  
Student | CSE (AI & ML) |
