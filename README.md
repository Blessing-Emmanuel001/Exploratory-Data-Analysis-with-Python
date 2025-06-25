# Car Insurance Analysis

## Table of Content

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tool](#tool)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)
  
## Project Overview

This project involves performing an exploratory data analysis(EDA) on an automobile dataset to uncover patterns, trends, and insights within the data. The primary goal is to understand the stucture and quality of the dataset, identify key variables, and evaluate their distribution and relationships.

## Data Source

Automobile Data: The primary dataset used for this analysis is the [automobile_dataset.csv](https://github.com/Blessing-Emmanuel001/Exploratory-Data-Analysis-with-Python/blob/main/automobile_dataset.csv) file containing detailed information about various cars including their technical specifications, insurance risk ratings and normalised loss values.

## Tool

Python

## Data Cleaning and Preparation

In the initial data preparation phase, I performed the following tasks:
- Data loading and inspection
- Detect columns or rows with missing values
- Drop row with missing values
- Fill missing numeric values with mean
- fill missing categorical data with mode
- Remove irrelevant columns
- Remove duplicates and inconsistencies
- Confirm data types

## Exploratory Data Analysis

EDA involves exploring the data to answer key questions such as:
1. What are the different car makes(brands) represented in the dataset and represent using a chart
2. What type of fuel (gas, diesel) and body styles(sedan, hatchbacks,etc) are most common 
3. What is the average price of a car in the dataset
4. Which car features are associated with higher risks (e.g., higher price, engine size, horsepower)?
5. Which cars are more likely to be owned by customers who value fuel efficiency (for eco-driving policies)?
6. Does vehicle weight (curb-weight) influence the likelihood or severity of damage in accidents?
7. How can price segmentation create premium categories (e.g., economy, mid-range, luxury)?
8. What is the cost difference between gas and diesel cars, and how should this affect policy pricing?
9. Which vehicle attributes suggest a higher likelihood of expensive repairs or replacement?
10. How can the company segment its vehicle-owning clients for better-targeted insurance offerings (e.g., young drivers, low-income drivers)?

## Data Analysis
#### View Full Jupyter Notebook

👉 [Click here to view the notebook in nbviewer](https://nbviewer.org/github/Blessing-Emmanuel001/Exploratory-Data-Analysis-with-Python/blob/main/eda_car_insurance_analysis.ipynb)

## Results

The analysis results are summarized as folllows:
1. Car Brands Represented: The dataset includes 22 unique car makes, such as Toyota, BMW, Audi, Honda, Mercedes-Benz, Porsche and more. Toyota is the most represented brand.
2. Most Common Fuel & Body Style: Fuel Type: Gas-powered vehicles dominate and for Body Style: Sedans are the most common body style.
3. Average Car Price: The average price of vehicles is approximately $13,207.
4. Features Associated with Higher Prices: Strong positive correlation with:
	•	Engine size (0.87)
	•	Curb weight (0.83)
	•	Horsepower (0.81)
	•	Vehicle width (0.75)
Vehicles with higher engine sizes and horsepower tend to be more expensive and risky. These include sports and luxury cars with higher insurance implications.
5. Top Fuel-Efficient Vehicles (Highway MPG):Brands like Honda, Toyota, and Volkswagen top the list in fuel efficiency (measured via highway MPG). Ideal for eco-conscious and cost-sensitive buyers.
6. Curb Weight vs Damage Severity: Heavier vehicles tend to have higher prices, potentially correlating with greater repair costs in accidents.
7. Price Segmentation: Vehicles segmented as:
	•	Economy: 98 cars (≤ $10,000)
	•	Mid-range: 78 cars ($10,001–$20,000)
	•	Luxury: 25 cars (>$20,000)
Helps target customers based on affordability.
8. Fuel Type & Cost Comparison: Diesel cars tend to be more expensive than gas cars. Can influence pricing models for fuel type.
9. Repair Cost Indicators: Vehicles with higher engine size, horsepower, and curb weight are more likely to incur expensive repairs or replacements.
10. Client Segmentation for Insurance:
	•	Using symboling (risk rating) to segment:
	•	Lower-risk cars (e.g., symboling -2, -1) have higher average prices
	•	Higher-risk cars (symboling 1–3) are typically less expensive

### Recommendations

Based on the Analysis results, here are some targeted recommendations. These can guide business decisions around marketing, pricing, policy design, insurance, and product segmentation:

1. Refine Product Segmentation
	•	Clearly define price-based vehicle categories (Economy, Mid-range, Luxury).
	•	Use these segments to tailor marketing, pricing tiers, and insurance packages.
2. Promote Fuel-Efficient Cars
	•	Highlight and promote highway-MPG vehicles like Honda, Toyota, and Chevrolet models to eco-conscious customers.
	•	Consider eco-friendly policies or incentives (e.g., discounts on fuel-efficient cars).
3. Develop Risk-Based Insurance Models
	•	Leverage the symboling score (risk rating) to offer tiered insurance premiums.
	•	High symboling = higher premium; low symboling = incentive for safe car choices.
4. Customize Maintenance Plans
	•	Vehicles with high engine size, horsepower, and curb weight should come with premium repair packages.
	•	Offer extended warranty or maintenance plans for these models.
5. Price Sensitivity by Fuel Type
	•	Since diesel vehicles are more expensive, consider:
	•	Higher insurance or tax rates for diesel.
	•	Subsidies or promotions for gas or hybrid cars in specific customer segments.
6. Use Curb Weight for Safety Classification
	•	Although curb-weight has a weak link to accident severity, it can still help create safety classes for regulatory or educational content.
7. Enhance Client Targeting
	•	Segment customers by vehicle type, income level, and fuel preference to send more relevant offers. For example:
Young drivers → Fuel-efficient, compact vehicles.
High-income clients → Luxury and performance-focused packages.
8. Optimize Inventory Strategy
	•	Keep more sedans and gas-powered vehicles in stock due to their popularity.
	•	Reduce or carefully manage inventory for rare body types or less efficient cars.
9. Policy Development for Repair Cost Recovery
	•	Offer premium insurance or repair add-ons for vehicles prone to higher repair costs (high engine size, horsepower, weight).
10. Customer Education & Tools
	•	Develop a car selection guide or web tool that helps customers balance between price, fuel efficiency, and repair cost risks.

### Limitations

1. Some features (e.g., normalized-losses) had missing values, which can affect the accuracy of insights.
2. Key customer-related attributes (e.g., age, income, location, driving habits) were missing, limiting personalized insights.
3. Variables like symboling were used as proxies for risk, and normalized-losses for damage severity, these may not reflect real-world outcomes accurately.
4. The dataset may not reflect current car prices, models, or market trends.
5. Estimations about expensive repairs were inferred using correlations, not actual maintenance cost data.
6. Detailed model or trim data (e.g., sport, hybrid, electric versions) were missing, reducing analysis depth.

### References

Pandas Documentation
Used for data cleaning, exploration, and analysis.
https://pandas.pydata.org/docs/

Kaggle – Automobile EDA Projects
Examples of similar automobile datasets and exploratory projects.
https://www.kaggle.com/

