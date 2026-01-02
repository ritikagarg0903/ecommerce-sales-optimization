## MarketPlace E-Commerce Sales Analysis And Optimization

---

## Case Narrative

### Company Background
MarketPlace is a rapidly growing online retailer that has established itself as a competitive player in the e-commerce market over the past five years. The company operates across three major product categories: **Electronics, Home Goods, and Fashion**. With over **200 product subcategories** and **monthly revenues exceeding $50 million**, MarketPlace has reached a critical juncture where **data-driven decision-making** is essential for sustained growth.

---

### Business Context
Tracy Martinez, the newly appointed **VP of Marketing Analytics**, is under pressure from the executive team to justify the company’s expanding **digital marketing budget**, which has increased by 40% year-over-year.  

- The **CFO** questions whether marketing spend is generating adequate returns  
- The **CMO** wants clarity on which factors truly drive sales performance  

Tracy’s analytics team has been asked to build a **predictive multiple regression model** to:

- Identify key drivers of monthly sales performance  
- Quantify the impact of marketing investments on revenue  
- Provide actionable insights for marketing budget allocation  
- Enable accurate sales forecasting for strategic planning  

---

## The Data

The dataset contains **18 months of sales data** across **200 product subcategories**, resulting in **3,600 monthly observations**.

### Response Variable
- **Sales**: Monthly sales revenue (in thousands of dollars)

### Continuous Predictors
- **Ad_Spend**: Monthly digital advertising spend (in thousands of dollars)  
- **Email_Campaigns**: Number of promotional email campaigns  
- **Website_Traffic**: Unique website visitors (in thousands)  
- **Avg_Rating**: Average customer rating (1–5 scale)  
- **Discount_Pct**: Average discount percentage  
- **Competitor_Price_Index**: Relative price index (100 = same price as competitors; >100 = cheaper; <100 = more expensive)  
- **Inventory_Level**: Average inventory units available  
- **Social_Media_Engagement**: Composite engagement score (0–100)

### Categorical Predictors
- **Season**: Winter, Spring, Summer, Fall  
- **Product_Type**: Electronics, Home, Fashion  

---

## Your Role
As a **senior data analyst** on Tracy’s team, you are responsible for building and interpreting a **multiple regression model** whose results will influence a **$20 million annual marketing budget allocation**.

---

## Part 1: Creating the Multiple Regression Model

### Dummy Variable Creation

#### Season
- Create dummy variables:
  - `Season_Spring`
  - `Season_Summer`
  - `Season_Fall`
- Use **Winter** as the reference category  
- Discuss why Winter may be an appropriate reference category  

#### Product Type
- Create dummy variables:
  - `Product_Type_Home`
  - `Product_Type_Fashion`
- Use **Electronics** as the reference category  
- Discuss why Electronics may be an appropriate reference category  

### Model 1: Full Model
Build a multiple regression model including:

**Continuous variables**
- Ad_Spend  
- Email_Campaigns  
- Website_Traffic  
- Avg_Rating  
- Discount_Pct  
- Competitor_Price_Index  
- Inventory_Level  
- Social_Media_Engagement  

**Dummy variables**
- Season_Spring  
- Season_Summer  
- Season_Fall  
- Product_Type_Home  
- Product_Type_Fashion  

Present a professional regression table including:
- Coefficients  
- Standard errors  
- t-statistics  
- p-values  

---

## Part 2: Test of Overall Model Validity

### Global F-Test
- State the null and alternative hypotheses  
- Interpret the hypotheses in business terms  

### Model Significance
- Report the F-statistic  
- Degrees of freedom (numerator and denominator)  
- p-value  
- Critical F-value at α = 0.05  

### Conclusion
- State the statistical conclusion  
- Interpret what this result means for Tracy’s team  
- Explain the business implications  

---

## Part 3: Test of Individual Coefficients

### Coefficient Table
Create a comprehensive table including:
- Variable name  
- Coefficient estimate  
- Standard error  
- t-statistic  
- p-value  
- Significance at α = 0.05  

### Advertising Effectiveness
For **Ad_Spend**:
- State the null and alternative hypotheses  
- Report the t-statistic and p-value  
- Make a statistical conclusion  
- Interpret the result for advertising effectiveness  

### Summary
- List statistically significant predictors  
- List non-significant predictors  
- Provide a concise business interpretation  

---

## Part 4: Interpreting Coefficients

### Ad_Spend
Interpret the coefficient:
> For every $1,000 increase in advertising spend, monthly sales change by $___ thousand, holding all else constant.

Discuss the return on ad spend and implications for marketing investment.

### Avg_Rating
- Interpret the coefficient in business terms  
- Discuss implications for customer satisfaction  

### Season_Summer
- Interpret relative to Winter  
- Discuss seasonal strategy implications  

### Product_Type_Fashion
- Interpret relative to Electronics  
- Discuss product strategy implications  

---

## Part 5: Model Selection (SE and Adjusted R²)

### Model 2
Build a reduced model using:
- Ad_Spend  
- Website_Traffic  
- Avg_Rating  
- Seasonal dummies  
- Product type dummies  

### Standard Error Comparison
- Compare SE for Model 1 and Model 2  
- Interpret implications for prediction accuracy  

### Adjusted R² Comparison
- Compare Adjusted R² values  
- Interpret model fit  

### Recommendation
Recommend a model for business decision-making based on:
- Statistical performance  
- Model simplicity  
- Strategic usability  

---

## Part 6: Prediction and Interval Estimation

### New Product Scenario
- Ad_Spend = 25  
- Email_Campaigns = 10  
- Website_Traffic = 150  
- Avg_Rating = 4.5  
- Discount_Pct = 15  
- Competitor_Price_Index = 105  
- Inventory_Level = 1,000  
- Social_Media_Engagement = 70  
- Season = Fall  
- Product_Type = Home  

### Point Prediction
- Calculate predicted monthly sales  
- Show the regression equation  

### Prediction Interval
- Compute and interpret a 95% prediction interval  
- Explain implications for operational planning  

### Confidence Interval
- Compute and interpret a 95% confidence interval for mean sales  
- Explain implications for strategic planning  

### Interval Comparison
- Explain why the prediction interval is wider  
- Describe when to use each interval with business examples  

---

## Part 7: Partial F-Test

### Marketing Investment Evaluation
Test whether the following variables are **jointly significant**:
- Ad_Spend  
- Email_Campaigns  
- Social_Media_Engagement  

### Hypotheses
- Define full and reduced models  
- State hypotheses mathematically and in business terms  

### Reduced Model
- Build the reduced model  
- Report R² and SSE  

### Partial F-Statistic
- Show calculation  
- Report F-statistic and p-value  

### Conclusion
- State the conclusion  
- Provide a recommendation to the CFO  

---

## Part 8: Coefficient of Partial Determination

### Reduced Model
- Use Model 1 as the full model  
- Report R² for the reduced model  

### Partial R²
- Calculate the coefficient of partial determination  

### Interpretation
Explain how much additional variance is explained by the three controllable marketing variables and whether they should remain in the model.

---

## Part 9: Dummy Variable Interpretation

### Seasonal Analysis
- Rank seasons from highest to lowest sales  
- Create a table showing sales adjustments relative to Winter  
- Compare Winter vs. Summer  
- Test whether Spring and Fall differ significantly  

### Product Type Analysis
- Rank product categories by sales  
- Calculate sales premiums/discounts relative to Electronics  
- Compare Home vs. Fashion and discuss investment strategy  

---

## Dataset Information
- **File**: `MarketPlace_Sales_Data.csv`  
- **Observations**: 3,600  
- **Time Period**: 18 months  
- **Variables**: 13 total  
