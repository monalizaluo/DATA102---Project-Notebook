# 🍽️ Fusion Cuisine Analysis Using Yelp Dataset

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Latest-brightgreen)](https://pandas.pydata.org/)
[![Dataset](https://img.shields.io/badge/Yelp-Open%20Dataset-red)](https://business.yelp.com/data/resources/open-dataset/)

## 🌟 Problem Statement

Fusion cuisine has become a popular culinary trend, combining components from several culinary traditions to create unique eating experiences.  Despite its popularity, data-driven research is scarce on what makes fusion restaurants successful in terms of customer happiness, company performance, and market placement.  Restaurant owners and entrepreneurs interested in this area encounter confusion about the best combinations of food kinds, restaurant qualities, pricing tactics, and customer-friendly service aspects.  The Yelp Open Dataset provides a unique opportunity to investigate these concerns by analyzing detailed business information and user-generated reviews.  This study intends to solve the difficulty of determining which fusion cuisine combinations are most well-received, how consumer sentiment connects with restaurant features, and what patterns emerge among successful fusion restaurants.  This study uses data mining techniques such as association rule learning, clustering, and classification to uncover actionable insights into consumer preferences and behavioral trends in the fusion cuisine segment, which will ultimately guide strategic menu development, pricing, and marketing decisions.

## 🎯 Objective

This project aims to analyze consumer behavior related to fusion cuisine by examining review sentiments, rating patterns, and visit frequencies. By identifying patterns in customer feedback and restaurant attributes, the study seeks to provide actionable insights for restaurant owners considering a fusion concept.

## 📊 Dataset

The study will utilize the [Yelp Open Dataset](https://business.yelp.com/data/resources/open-dataset/)

The dataset includes:
- `business.json` – Detailed business information (categories, location, attributes, etc.)
- `review.json` – User reviews, ratings, and review text

## 🔍 Relevance for Fusion Cuisine

- **Identifying Fusion Restaurants**: Filtering Yelp's business JSON to identify fusion cuisine restaurants using categories and descriptive text (e.g., "Asian Fusion")
- **Behavioral Data Analysis**: Utilizing review JSON for ratings and textual feedback to understand customer sentiment and engagement

## �� Data Mining Problems & Techniques

### 1. Association Rule Learning
- **Objective**: Identify common attribute combinations among highly rated fusion restaurants
- **Example**: Restaurants with "Asian" and "Latin" fusion and a casual atmosphere have higher customer satisfaction

### 2. Clustering
- **Objective**: Segment fusion restaurants based on cuisine combinations, pricing, and review sentiment scores
- **Example**: Differentiating clusters of budget-friendly vs. premium fusion establishments

### 3. Classification/Regression
- **Objective**: Predict restaurant success (e.g., likelihood of high ratings) based on features and menu composition
- **Example**: Using cuisine diversity, price range, and review count to classify restaurants as "successful" or "underperforming"

## 🛠️ Data Collection and Processing

<details>
<summary>Click to expand Data Collection details</summary>

### Data Collection
- Download the Yelp Open Dataset (JSON format)

### JSON Parsing & Preprocessing
- Use Python's json and pandas libraries for data parsing
- Convert JSON files into structured DataFrames
- Handle missing/inconsistent values in key fields like categories and price ranges

### Data Integration & Feature Engineering
- Merge business and review datasets using business_id
- Filtering Fusion Restaurants: Use keywords to create binary flags for fusion classification
- Review Metrics Aggregation: Compute average ratings, review count, and sentiment scores using lexicon-based approaches
- Data Transformation: Encode categorical variables and normalize numerical features
</details>

## 📈 Modeling and Evaluation

<details>
<summary>Click to expand Modeling details</summary>

### Association Rule Mining
- Apply Apriori algorithm to identify frequent attribute combinations

### Clustering
- Use k-means or hierarchical clustering to segment fusion restaurants

### Classification/Regression
- Develop predictive models (e.g., decision trees, logistic regression)

### Evaluation Metrics
- Classification: Accuracy, precision, recall
- Clustering: Silhouette score
- Regression: Mean squared error (MSE)
</details>

## 🔬 Hypotheses

1. **Distinct Attribute Patterns**: Fusion restaurants with specific cuisine pairings will exhibit distinct attribute patterns correlated with high ratings
2. **Cluster Differentiation**: Clustering will reveal market segments, each with unique customer behavior
3. **Predictive Success**: A classification model can reliably predict restaurant success based on features

## ✨ Novelty & Feasibility

### Novelty
- Fusion cuisine is an emerging niche in the food industry, with limited data-driven studies
- Integrates consumer behavior analysis with traditional data mining techniques

### Feasibility
- JSON data can be efficiently processed using Python libraries
- Proposed techniques align with standard classroom topics

## 🎯 Conclusion

This project will provide a data-driven perspective on fusion cuisine's market dynamics using Yelp data, offering actionable insights for restaurant owners, chefs, and industry analysts. By uncovering key sentiment patterns, pricing correlations, and cuisine pairings that drive customer satisfaction, our findings can guide strategic decisions on menu innovation, pricing strategies, and marketing approaches.

Additionally, this study contributes to the broader understanding of consumer behavior in niche dining markets, demonstrating the power of data mining in real-world applications. Beyond academic relevance, the project aligns with evolving industry trends, equipping restaurateurs with the analytical tools needed to thrive in an increasingly competitive and experience-driven food industry.

---
<div align="center">

📊 **Project Status**: In Progress

</div>
