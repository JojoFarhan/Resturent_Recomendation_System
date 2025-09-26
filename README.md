# 🍽️ Restaurant Recommendation by Food Review Dataset

This project builds a **restaurant recommendation system** using food review data from Bangladesh.  
It leverages **NLP, sentiment analysis, machine learning, and deep learning** techniques to recommend restaurants based on customer reviews.

---

## 📌 Features
- Load and preprocess restaurant review dataset  
- Perform **sentiment analysis** on reviews using Hugging Face Transformers  
- Calculate **mean restaurant ratings** (scaled between 1–5)  
- Visualize:
  - Distribution of restaurant ratings  
  - Top 10 rated restaurants  
  - Sentiment distribution across reviews  
  - Most famous restaurant chains  
  - Word frequency distributions from reviews  
- Build a **TF-IDF & Cosine Similarity based recommendation system**  
- Provide two types of recommendations:
  1. **Similar restaurants** (based on review similarity)  
  2. **Location-based recommendations** (similar restaurants in the same city)

---

## 🛠️ Tech Stack
- **Python Libraries**:  
  - Data Handling: `numpy`, `pandas`, `scipy`  
  - Visualization: `matplotlib`, `seaborn`  
  - NLP: `nltk`, `transformers` (Hugging Face)  
  - Machine Learning: `scikit-learn`  
  - Deep Learning: `tensorflow`, `keras`  
  - Utilities: `tqdm`, `pickle`, `gc`, `warnings`
- **Sentiment Analysis Model**: Hugging Face `pipeline("sentiment-analysis")`  
- **Platform**: Google Colab (with Google Drive integration)

---

## 📂 Dataset
- **File**: `Food Review Dataset of Bangladesh.xlsx`  
- **Sheet**: `Sheet1`  
- Columns used:  
  - `restaurant`, `city`, `preprocessed_text`, `ratings_int`  
- Preprocessing includes:
  - Dropping unnecessary columns (`reviewer_name`, `ratings`, `review_text`, etc.)  
  - Removing nulls & duplicates  
  - Sampling ~8300 reviews  

---

## 📊 Visualizations
- Restaurant rating distribution  
- Top 10 restaurants  
- Sentiment distribution pie chart  
- Most famous restaurants (chains)  
- Word couple frequency plots  

---

## 🤖 Recommendation System
### 🔹 Recommend Similar Restaurants
```python
recommend("Kacchi Bhai - Dhanmondi")
recommend("Barcode Cafe_Chittagong")

### 🔹 Recommend Restaurants by Location
recommend_by_location("Kacchi Bhai - Dhanmondi")
recommend_by_location("Barcode Cafe_Chittagong")
🚀 How to Run

Clone this repository
Open the notebook in Google Colab
Mount Google Drive:

from google.colab import drive
drive.mount('/content/drive')


Update dataset path:
XLSX = '/content/drive/MyDrive/Colab Notebooks/Food Review Dataset of Bangladesh.xlsx'
Run all cells to preprocess data, analyze sentiments, visualize insights, and generate recommendations.

## 📈 Future Improvements

Deploy as a web app using Streamlit or Flask
Enhance recommendation system using deep learning embeddings
Incorporate user preferences for personalized results
Expand dataset to cover more restaurants and cities

## 📜 License
This project is for educational and research purposes only.
Dataset rights belong to the original source.

👨‍💻 Developed with ❤️ using Python & NLP
