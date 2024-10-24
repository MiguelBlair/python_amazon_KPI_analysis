# Python Amazon KPI Analysis

## Project Overview

In this project, I focused on analyzing e-commerce data from Amazon, a leading industry player, to uncover key insights that could optimize strategies for new and aspiring e-commerce businesses. By analyzing sales data, I aimed to understand trends that are invaluable for decision-making and business growth.

## Data Collection

The dataset used for this analysis was scraped from Amazon's site by [Ahmed Abdelrazek](https://www.kaggle.com/datasets/ahmedsayed564/amazon-sales-dataset). The initial data preview helped identify potential key insights and necessary data cleaning steps.

### Dataset Overview
- **Total Rows:** 1465
- **Total Columns:** 16
- **Key Columns:**
  - `product_id`
  - `product_name`
  - `category`
  - `discounted_price`
  - `actual_price`
  - `discount_percentage`
  - `rating`
  - `rating_count`
  - `review_content`

## Libraries Used

- **Pandas:** For data loading, cleaning, and preliminary analysis.
- **NumPy:** For mathematical operations and handling arrays.
- **Matplotlib:** For basic plotting and visualizations.
- **Seaborn:** For detailed and visually appealing charts.

## Data Cleaning

The data was cleaned by:
- Removing duplicate rows
- Dropping irrelevant columns
- Handling strange entries (e.g., replacing invalid ratings)
- Converting data types for easier analysis

## Key Insights & Visualizations

### 1. Relationship between Discounts and Product Ratings
- Analyzed how discount percentages correlate with product ratings.
- Visualized using a scatter plot with a regression line.
- **Correlation Coefficient:** -0.15 (weak negative correlation)

### 2. Highest-Rated Product Categories
- Investigated which product categories received the highest ratings.
- Created a bar graph displaying the top 5 categories by average rating.
- **Top Categories:**
  1. Computers & Accessories | Tablets - Average Rating: 4.6
  2. Office Products | Office Electronics | Calculators | Books - Average Rating: 4.5
  3. Home & Kitchen | Kitchen & Home Appliances | Small Kitchen Appliances - Average Rating: 4.5

### 3. Impact of Discounts on the Number of Reviews
- Explored how discounts influence customer engagement.
- Analyzed correlation between discount percentage and number of reviews.
- **Correlation Coefficient:** 0.01 (very weak positive relationship)

### 4. Price Distribution of Highly-Rated Products
- Examined the price ranges of products with the highest ratings (rating ≥ 4).
- Visualized the distribution of discounted prices for highly-rated products.
- **Statistics:**
  - Mean Discounted Price: ₹X.XX
  - Median Discounted Price: ₹X.XX
  - Mode Discounted Price: ₹X.XX

## Conclusion

The analysis revealed that discounts do not have a significant impact on product ratings, while certain categories consistently receive higher ratings. Additionally, higher discounts may not always translate to more reviews, indicating that customer engagement is influenced by multiple factors.

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/repository-name.git
   cd repository-name
   ```

2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```

3. Run the analysis:
   ```python
   python amazon_kpi_analysis.py
   ```
