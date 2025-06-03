# AI-POWERED FAKE NEWS DETECTION SYSTEM
## Combating Misinformation with NLP and Machine Learning for a More Informed Digital Society
![image](https://github.com/user-attachments/assets/80b0af64-2b20-4ed0-8b9e-5fb21ced8661)

***⚠️ Disclaimer:** This project is based on a publicly available dataset for educational purposes only. It demonstrates my ability to build end-to-end NLP and machine learning pipelines to address real-world challenges like misinformation detection.*

## INTRODUCTION  
In today's digital world, misinformation spreads faster than ever. This project presents a machine learning-powered **Fake News Detection System** that analyzes news articles and classifies them as *real* or *fake*. By combining natural language processing (NLP) with ensemble learning techniques, this tool can assist media organizations, platforms, and fact-checking services in identifying misleading information automatically.

---

## PROBLEM STATEMENT  
With the growing volume of online news, it's nearly impossible to manually fact-check every story. This project aims to build an intelligent, scalable, and interpretable model that classifies news articles based on their content and metadata using supervised learning.

---

## METHODOLOGY

1. **Data Cleaning & Preparation**  
   - Merged `title` and `text` fields.  
   - Extracted time-based features (`year`, `month`, etc.).  
   - Removed duplicates and missing entries.

2. **Exploratory Data Analysis (EDA)**  
   - Visualized class distributions and trends over time.  
   - Identified common subjects (e.g., Politics, World News) in fake vs. real articles.

3. **Feature Engineering**  
   - Applied **TF-IDF vectorization** to convert text into numerical features.  
   - Label-encoded categorical data (`subject`).  
   - Engineered features from dates to detect publication patterns.

4. **Handling Class Imbalance**  
   - Used **RandomUnderSampler** and **SMOTE** for class balance.  
   - Applied **Stratified K-Fold** to avoid bias in training/testing splits.

5. **Model Training & Evaluation**  
   - Trained models: `LogisticRegression`, `XGBoostClassifier`, and `VotingClassifier`.  
   - Evaluated using accuracy, F1-score, confusion matrix, ROC-AUC.  
   - Addressed **overfitting** by tuning regularization and performing cross-validation.

---

## TOOLS & TECHNOLOGIES

| Tool/Library         | Purpose                                   |
|----------------------|--------------------------------------------|
| Python               | Core programming language                 |
| Pandas, NumPy        | Data preprocessing and manipulation       |
| Matplotlib, Seaborn  | Data visualization and EDA                |
| Scikit-learn         | ML models and preprocessing               |
| XGBoost              | Gradient-boosted decision trees           |
| VotingClassifier     | Ensemble model for improved performance   |
| TF-IDF               | Text vectorization                        |
| Jupyter Notebook     | Development environment                   |

---

## KEY INSIGHTS

- Most fake news spiked in **mid-2016**, aligning with real-world political events.
- Categories like **Politics** and **World News** were commonly misused for fake headlines.
- Time-based features helped in spotting seasonal misinformation trends.
- **Ensemble models** delivered better generalization than individual classifiers.

---

## REAL-WORLD IMPACT

This system can be adapted by:

- **Social Media Platforms**: Automatically flag suspicious news stories.  
- **News Aggregators**: Filter and prioritize credible articles.  
- **Fact-Checking Agencies**: Identify high-risk content for human review.  
- **Media Literacy Programs**: Educate the public with data-driven insights into misinformation trends.

---

## FUTURE ENHANCEMENTS

- Integrate **BERT** or **RoBERTa** for deep contextual understanding.  
- Build an **interactive web app** using Streamlit or Flask.  
- Add a **credibility scoring system** with explainable AI (e.g., SHAP).  
- Enable **multilingual fake news detection**.  
- Personalize detection based on user interest and past behavior.

---
