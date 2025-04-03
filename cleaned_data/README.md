# Data Cleaning Process Documentation

## Overview
This folder contains the cleaned and processed data files from the Yelp Dataset, specifically focused on fusion restaurants and their reviews.

## Files
- `fusion_restaurants.csv`: Contains cleaned data about fusion restaurants including business details, ratings, and attributes

## Data Cleaning Steps

### 1. Initial Data Loading
- Loaded the original Yelp JSON dataset
- Focused on business.json and review.json files
- Used pandas for data processing

### 2. Business Data Cleaning
1. **Filtering Restaurants**
   - Identified restaurants using the 'categories' field
   - Selected businesses with 'Restaurants' in their categories

2. **Identifying Fusion Restaurants**
   - Created `is_fusion` flag based on categories containing 'Asian Fusion' or other fusion-related terms
   - Added `is_restaurant` boolean field

3. **Handling Missing Values**
   - Filled missing numerical values with appropriate defaults
   - Processed JSON-formatted attribute strings into structured data
   - Standardized business hours format

4. **Feature Engineering**
   - Extracted price range from attributes
   - Calculated average ratings
   - Computed review counts
   - Generated sentiment scores from review text

### 3. Data Standardization
- Normalized business categories
- Standardized price ranges (1-4 scale)
- Formatted geographical coordinates
- Cleaned and standardized address fields

### 4. Final Processing
- Merged business and review data
- Calculated aggregate metrics
- Removed duplicate entries
- Exported to CSV format

## Column Descriptions

- `business_id`: Unique identifier for each business
- `name`: Business name
- `address`: Physical location
- `city`, `state`, `postal_code`: Location details
- `latitude`, `longitude`: Geographical coordinates
- `stars`: Overall rating (1-5)
- `review_count_x`: Number of reviews from business data
- `is_open`: Whether business is operational (1) or closed (0)
- `attributes`: Business characteristics (JSON format)
- `categories`: Business categories
- `hours`: Operating hours
- `is_restaurant`: Boolean flag for restaurant classification
- `is_fusion`: Boolean flag for fusion cuisine
- `price_range`: Price level (1-4)
- `avg_rating`: Average rating from reviews
- `review_count_y`: Number of reviews from review data
- `rating_std`: Standard deviation of ratings
- `avg_sentiment`: Average sentiment score from review text

## Data Quality Metrics
- No missing values in key fields
- Consistent data types across columns
- Validated geographical coordinates
- Verified business categories
- Checked price range consistency

## Usage Notes
- All timestamps are in local time zones
- Price ranges: 1 ($) to 4 ($$$$)
- Ratings are on a 1-5 scale
- Sentiment scores range from -1 to 1

## Dependencies
- Python 3.7+
- pandas
- numpy
- textblob (for sentiment analysis)
