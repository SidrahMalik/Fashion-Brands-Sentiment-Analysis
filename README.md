# 🧵 Sentiment Analysis of Pakistani Fashion Brands

This project analyzes customer perceptions of major Pakistani fashion brands like **Khaadi**, **Gul Ahmed**, and **Sapphire** by using sentiment analysis techniques on customer comments.

## 📌 Objective

To understand how customers feel about Pakistani clothing brands and what drives those sentiments—using data-driven analysis, visualizations, and natural language processing techniques.

---

## 🛠️ Tools & Technologies

| Purpose | Tool / Library |
|--------|----------------|
| Data Analysis | `pandas`, `numpy` |
| Text Cleaning | `re`, `string`, `nltk` |
| Sentiment Analysis | `TextBlob` |
| Visualization | `matplotlib`, `seaborn` |
| Word Frequency | `collections.Counter`, `wordcloud` |
| Temporal Analysis | `pandas datetime`, `matplotlib` |
| Scraping (attempted) | `snscrape` (Twitter scraping - failed due to timeout) |

---

project-root/
├── brand_reviews.csv # Raw dataset containing user comments and brand names
├── cleaned_brand_reviews.csv # Dataset after text preprocessing and cleaning
├── brand_reviews_with_sentiment.csv # Final dataset with sentiment labels and synthetic date column
├── sentiment_analysis.ipynb # Jupyter Notebook containing all analysis and visualizations
└── README.md # Project documentation (this file)

---

## 🧪 Steps Performed

### ✅ Phase 1: Data Preparation
- Original data was scraped manually and supplemented using a CSV file.
- Cleaned text using lowercase conversion, punctuation removal, stopwords removal, etc.
- Added a synthetic `date` column (random dates from Jan–Mar 2024) for temporal analysis.
- Applied `TextBlob` to assign sentiment: **Positive**, **Negative**, or **Neutral**.

### ✅ Phase 2: Sentiment Visualization
- **Pie chart** and **bar chart** showing distribution of sentiments across all comments.
- **Line graph** showing sentiment trends over time (by month).

### ✅ Phase 3: Customer Perception Insights
- Created **word clouds** of frequently used terms in positive and negative comments.
- Analyzed how sentiment changes over time.
- Identified key sentiment drivers such as "quality", "delivery", "customer service".

---

## 📊 Sample Visualizations

- Pie chart of sentiment distribution
- Monthly line graph showing sentiment change
- Word clouds for positive and negative sentiments
- Sentiment comparison before and after mock campaign date

---

## 💡 Future Improvements

- Use real timestamps from social media platforms
- Integrate more robust sentiment models like BERT or VADER
- Correlate sentiment trends with actual marketing campaigns and events


