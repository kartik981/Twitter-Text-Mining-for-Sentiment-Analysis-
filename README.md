# Twitter Text Mining for Sentiment Analysis and Like Prediction

## Introduction
Social media platforms provide valuable insights into public sentiment and trends. This project applies **text mining** on Donald Trump’s tweets to:
- Perform **sentiment analysis**.
- Predict **tweet popularity** (number of likes) using machine learning models.

## Methodology
### Data Preprocessing
1. **Data Selection:**
   - Focused on tweets from **2014 to 2020**.
   - Removed tweets with fewer than **five words**.
2. **Text Cleaning:**
   - Tokenized text and removed **special characters**.
   - Filtered out **stopwords and internet jargon** (e.g., ‘http’, ‘rt’).
   - Converted text to **lowercase** for uniformity.
3. **Final Dataset:** **31,077 processed tweets** ready for analysis.
### Visualizations
![Word Cloud](https://github.com/kartik981/Twitter-Text-Mining-for-Sentiment-Analysis-/blob/40d83febd026464f6ffb466edbeb1646dcc2d718/Word%20Cloud.png)
![Tweet Frequency](https://github.com/kartik981/Twitter-Text-Mining-for-Sentiment-Analysis-/blob/40d83febd026464f6ffb466edbeb1646dcc2d718/Tweet%20Freq.png)
![Trigrams](https://github.com/kartik981/Twitter-Text-Mining-for-Sentiment-Analysis-/blob/40d83febd026464f6ffb466edbeb1646dcc2d718/Trigrams.png)
![Quadgrams](https://github.com/kartik981/Twitter-Text-Mining-for-Sentiment-Analysis-/blob/40d83febd026464f6ffb466edbeb1646dcc2d718/Quadgrams.png)

### Sentiment Analysis
- **VADER Sentiment Analysis:**
  - Measures **positive, negative, and neutral sentiment**.
  - Provides a **compound sentiment score** for each tweet.
- **Key Findings:**
  - Tweets containing *“Make America Great Again”* had a **high positive sentiment**.
  - Tweets mentioning *“fake news”* had **strong negative sentiment**.

### Machine Learning for Like Prediction
#### Feature Engineering
- **Tweet Length**: Number of words per tweet.
- **TextBlob Sentiment Scores**: **Polarity** and **subjectivity**.
- **VADER Compound Score**: Overall sentiment value.
- **Retweets**: Influence of retweets on like count.

#### Model Performance
| Model                     | Accuracy  |
|---------------------------|-----------|
| Random Forest Regression  | 72.61%    |
| Linear Regression         | 71.54%    |
| Gaussian Naïve Bayes      | Poor Performance |

## Results & Discussion
- **Patriotic and controversial tweets received the most engagement.**
- **Trump’s Twitter activity was higher before and after his presidency.**
- **Random Forest performed best for like prediction**, while Gaussian Naïve Bayes was unsuitable due to high variance.

## Conclusion
The study demonstrates how businesses and organizations can use **Twitter text mining** for **insights into public sentiment and engagement**. Future improvements include:
- **Enhancing sarcasm detection** to improve sentiment accuracy.
- **Incorporating user profile data** for personalized analysis.
- **Ethical considerations** in handling social media data.

## Tools Used
- **Python (NLTK, TextBlob, scikit-learn, Matplotlib, Seaborn)**
- **Machine Learning Models: Random Forest, Linear Regression, Naïve Bayes**
- **Data Visualization: Word Clouds, Heatmaps, Sentiment Graphs**

## References
- Jockers, M. (2017). *Text Analysis with R for Students of Literature.*
- Hutto, C., & Gilbert, E. (2014). *VADER: A Parsimonious Rule-Based Model for Sentiment Analysis.*
- Twitter Developer Documentation (2022).
