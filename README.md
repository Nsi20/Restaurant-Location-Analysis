# Restaurant-Location-Analysis
Objective: Perform a geographical analysis of the restaurants in the dataset.

---

This project comprehensively analyses restaurant locations, including concentration, ratings, cuisine popularity, price ranges, and service options. It uses Python libraries such as Pandas, Plotly, and Geopandas to uncover insights into restaurant density, average ratings, cuisine trends, and location-based service preferences. The goal is to identify patterns that could guide strategic decisions for restaurant businesses, such as potential expansion areas, customer preferences, and pricing strategies.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Project Structure](#project-structure)
5. [Analysis and Insights](#analysis-and-insights)
6. [Results and Visualizations](#results-and-visualizations)
7. [Contributing](#contributing)
8. [License](#license)

---

## Project Overview

This project analyzes restaurant data to uncover patterns and insights across various locations. By grouping data by city or locality and calculating metrics like average ratings, common cuisines, and price ranges, we aim to provide valuable insights into restaurant distribution and characteristics. These insights can guide decisions in restaurant management, marketing, and expansion.

Key features include:
- Mapping restaurant concentrations by city or locality
- Identifying popular cuisines by region
- Analyzing the correlation between price range and ratings
- Visualizing high-rated restaurant clusters on a map
- Determining customer preferences for service options by city

## Dataset

The dataset contain information on restaurants, including the following columns:
- **City**: City where the restaurant is located
- **Locality**: Detailed location of the restaurant within the city
- **Aggregate rating**: Average rating given to the restaurant
- **Cuisines**: Types of cuisine served at the restaurant
- **Price range**: Price range category
- **Has Table booking**: Indicates if the restaurant offers table booking
- **Has Online delivery**: Indicates if the restaurant offers online delivery
- **Latitude** and **Longitude**: Geographic coordinates of the restaurant

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/nsi20/restaurant-location-analysis.git
   cd restaurant-location-analysis
   ```

2. **Install required libraries**:
   Use the following command to install necessary dependencies.
   ```bash
   pip install pandas plotly geopandas
   ```

3. **Set up Google Colab (optional)**:
   You can also run this project on Google Colab. To do this, upload the dataset to Colab and run the code provided in the project notebook.

## Project Structure

```
restaurant-location-analysis/
├── data/
│   └── dataset.csv               # Restaurant dataset file
├── analysis/
│   ├── city_concentration.py      # Analysis of restaurant concentration
│   ├── cuisine_analysis.py        # Cuisine popularity by location
│   ├── price_rating_correlation.py # Price range and rating correlation
│   └── service_options_analysis.py # Analysis of customer service preferences
├── visualizations/
│   ├── concentration_map.ipynb    # Mapping high-rated restaurants
│   └── correlation_scatter.ipynb  # Scatter plot for price and rating
├── README.md
└── LICENSE
```

## Analysis and Insights

This project explores the following insights:

### 1. High-Concentration Areas with Low Competition
   - Identify cities with a high restaurant count, but also find locations with few restaurants but high ratings, where competition is lower.
   - **File**: `analysis/city_concentration.py`

### 2. Popular Cuisines by Region
   - Understand regional cuisine preferences, useful for businesses exploring which cuisines to introduce based on location.
   - **File**: `analysis/cuisine_analysis.py`

### 3. Correlation Between Price Range and Ratings by City
   - Evaluate if there’s a correlation between price and ratings, helping businesses decide on appropriate pricing strategies.
   - **File**: `analysis/price_rating_correlation.py`

### 4. Clustering of Highly Rated Restaurants on a Map
   - Visualize clusters of high-rated restaurants to reveal “premium zones.”
   - **File**: `visualizations/concentration_map.ipynb`

### 5. City-Based Preferences for Service Options
   - Discover customer preferences for services like table booking and online delivery by city.
   - **File**: `analysis/service_options_analysis.py`

## Results and Visualizations

Each analysis step generates visualizations to illustrate the findings. Here’s an overview:

- **Restaurant Concentration by City**: Bar chart showing cities with the highest restaurant count.
- **Cuisine Popularity by City**: Displays the most common cuisines by city.
- **Price Range and Ratings Correlation**: Scatter plot to assess correlation between pricing and rating by city.
- **High-Rated Restaurant Clusters**: Map visualization showing clusters of high-rated restaurants.
- **Service Options Preferences**: Bar chart showing the popularity of service options (e.g., table booking) in various cities.

## Running the Project

To run the analysis locally:

1. Open the `.py` files in the `analysis/` folder and run them sequentially to explore different insights.
2. To visualize geographic data, open the `.ipynb` files in the `visualizations/` folder.
3. Ensure you update file paths if running the project in different environments (e.g., Google Colab).

### Example Run (Google Colab)

If using Google Colab, run the following code to upload your dataset and proceed with the analysis:

```python
from google.colab import files
import pandas as pd

uploaded = files.upload()
data = pd.read_csv(list(uploaded.keys())[0])
```

You can then continue with the provided code snippets for each section.

## Contributing

If you’d like to contribute:
1. Fork the repository.
2. Make your modifications.
3. Submit a pull request.

