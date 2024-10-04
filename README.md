# Hotel Reviews Analysis

This project focuses on analyzing a dataset containing over 515,000 guest reviews and ratings for approximately 1,500 hotels across Europe. The dataset was sourced from Booking.com and includes detailed customer feedback on various hotel aspects.

### Dataset Overview:
- **Number of Reviews**: 515,000+
- **Number of Hotels**: ~1,500 hotels
- **Location**: Hotels across Europe
- **Data Source**: [Kaggle Dataset - 515k Hotel Reviews in Europe](https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe)

The dataset consists of customer reviews and ratings along with hotel information, reviewer details, and other metadata. Text data in the reviews was cleaned by removing unicode characters, punctuation, and converting all text to lowercase. No additional preprocessing steps were performed on the data.

---

## Goals of the Analysis:

### 1. **Identify Top Hotel Features from Positive and Negative Reviews**:
   - **Objective**: Determine the top five features (e.g., location, staff, cleanliness, etc.) mentioned in the most positive and most negative reviews.
   - **Analysis Requirement**: Ensure the identified features are valid aspects of a hotel experience. Generic words such as "great" or "bad" should not be counted as features.

### 2. **Identify Features Based on Customer Type**:
   - **Objective**: Identify the top five features that customers prefer based on their travel category (e.g., solo traveler, group traveler, business trip, leisure trip, couple, family with children).
   - **Tags**: The analysis will focus on travel categories listed in the "Tags" column. Categories that are not needed will be excluded from the analysis.

### 3. **Country-Specific Feature Analysis**:
   - **Objective**: Identify the top five features that customers like and complain about in hotels located in four countries: the United Kingdom, France, Italy, and Spain.
   - **Field Used**: The hotel address field, `Hotel_Address`, will be used to extract country information for this analysis.

### 4. **Dashboard Creation**:
   Create a visual dashboard with the following plots:
   - **Top Five Hotels Overall**: Hotels with consistently high average ratings.
   - **Bottom Five Hotels Overall**: Hotels with consistently low average ratings.
   - **Five Most Improved Hotels**: Hotels with the highest improvement in average ratings between 2015 and 2017, showing average ratings for each year.

---

## Data Fields:
- **Hotel_Name**: Name of the hotel.
- **Reviewer_Score**: The numerical score given by the reviewer.
- **Review_Date**: Date of the review.
- **Tags**: Categorical labels such as solo traveler, group traveler, business trip, etc.
- **Review_Year**: Extracted year from the review date.
- **Hotel_Address**: The address of the hotel, including the country.
- **Positive_Review**: The text of the positive review.
- **Negative_Review**: The text of the negative review.

---

## Tools and Libraries Used:
- **Pandas**: For data cleaning, manipulation, and analysis.
- **Seaborn/Matplotlib**: For data visualization.
- **Plotly/Dash**: For creating interactive visual dashboards.

---

## Instructions to Run:
1. **Prerequisites**: Ensure you have Python 3.x installed along with the required libraries:
   - Pandas
   - Seaborn
   - Matplotlib
   - Plotly
   - Dash

2. **Running the Dashboard**:
   - Install the necessary libraries if they are not already available using:
     ```bash
     pip install pandas seaborn matplotlib plotly dash
     ```
   - Run the Python script provided in the notebook to launch the Dash app locally.
   - Once the app is running, open the provided localhost link in a web browser to view the interactive dashboard.

---

## Conclusion:
This project provides a comprehensive analysis of hotel reviews in Europe by focusing on identifying key features that customers value or complain about. The dashboard provides an interactive experience to visualize the top and bottom hotels and observe improvements in hotel ratings over time.
