E-commerce Funnel & Conversion Analysis
Overview

This project analyzes 500,000+ e-commerce user interactions from an online cosmetics dataset to examine customer behavior across the purchasing funnel and evaluate differences in conversion performance across brands.

The analysis focuses on two main questions:

Where does customer activity decline throughout the purchasing process?
Does higher product visibility correspond to higher conversion rates?
Analysis

Using R and tidyverse, I cleaned and aggregated behavioral event data including product views, cart additions, cart removals, and purchases.

I then:

Analyzed the distribution of user activity across funnel stages
Calculated brand-level purchase conversion rates
Compared conversion performance among high-traffic brands
Visualized the relationship between traffic volume and conversion
Used linear regression to test whether higher view counts predict higher conversion rates

To reduce misleading conversion estimates from low-traffic brands, conversion comparisons were restricted to brands exceeding minimum view thresholds.

Key Findings
Higher visibility did not reliably translate into higher conversion.
A regression of conversion rate against log-transformed views produced R² = 0.0845, meaning view volume explained only about 8.5% of the variation in conversion rates.
The relationship was not statistically significant (p = 0.335).
Some lower-traffic brands achieved stronger conversion performance than brands receiving substantially more views.
Event counts showed substantially fewer purchases than views and cart interactions, indicating an opportunity for deeper funnel analysis around the final stages of the purchasing process.
Technologies

R · tidyverse · ggplot2 · ggrepel · scales · Linear Regression

Methods
Data cleaning and filtering
Exploratory data analysis
Funnel analysis
Data aggregation
Conversion-rate analysis
Data visualization
Log transformation
Linear regression
