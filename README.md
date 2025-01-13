# Amazon Video Games Dataset Analysis

## Overview
This project performs data analysis on the [Amazon Video Games dataset](https://snap.stanford.edu/data/web-Amazon.html). The analysis includes statistical trend exploration, sentiment analysis, and a simple prediction model to classify reviews. It leverages Python and various data visualization and machine learning tools to uncover insights and trends within the dataset.

## Dataset Description
The dataset contains product reviews and metadata for the video games category on Amazon. Key fields analyzed include:
- Product Ratings (`overall`)
- Verification Status (`verified`)
- Review Text (`reviewText`)
- Review Dates (`reviewTime` and `unixReviewTime`)

## Key Features
### Data Cleaning and Preprocessing
- Handled missing values and verified data consistency.
- Parsed and converted timestamps for trend analysis.
- Extracted year information from review dates for time-series analysis.

### Exploratory Data Analysis (EDA)
- **Verification Analysis:** Visualized verification status distribution.
- **Ratings Analysis:** Explored the distribution of product ratings over the years.
- **Trend Analysis:** Analyzed average ratings trends over time.
- **Word Clouds:** Created visualizations for common review summaries.

### Sentiment Analysis
- Used NLTK's Sentiment Intensity Analyzer to classify reviews as positive, neutral, or negative.
- Visualized sentiment trends for different rating categories.

### Predictive Modeling
- Built a simple linear regression model to predict trends in ratings over the years.
- Experimented with decision tree classification for binary sentiment classification (positive/negative).

## Key Findings
- The average rating trend remained stable with minor fluctuations across years.
- Verified reviews accounted for the majority of the dataset.
- Word clouds highlighted popular themes and sentiments in user reviews.
- Linear regression indicated a slight positive trend in ratings over recent years.

## Technologies Used
- **Programming Languages:** Python
- **Libraries:**
  - `pandas` for data manipulation.
  - `matplotlib` and `seaborn` for data visualization.
  - `nltk` for sentiment analysis.
  - `scikit-learn` for predictive modeling.
  - `WordCloud` for visual representation of text data.

## How to Run
1. Clone the repository and download the dataset from [here](https://snap.stanford.edu/data/web-Amazon.html).
2. Ensure Python 3.x is installed with the required libraries:
   ```bash
   pip install pandas matplotlib seaborn nltk scikit-learn wordcloud
   ```
3. Run the Python script to reproduce the analysis:
   ```bash
   python analysis_script.py
   ```

## Visualizations
- **Verification Distribution:** Pie chart showing the percentage of verified and unverified reviews.
- **Ratings Distribution:** Bar chart showing the frequency of different ratings.
- **Yearly Trends:** Line plot displaying average ratings over the years.
- **Sentiment Analysis:** Bar plots visualizing sentiment scores for different ratings.
- **Word Clouds:** Text visualizations highlighting frequently used terms in reviews.

## Future Work
- Expand the classification model to include multiclass sentiment analysis.
- Integrate additional features from the dataset for improved predictions.
- Deploy the analysis results as an interactive dashboard.

## Acknowledgments
- **Dataset:** Provided by [Stanford Network Analysis Project (SNAP)](https://snap.stanford.edu).
- **Libraries:** Open-source Python libraries including `pandas`, `matplotlib`, and `nltk`.
