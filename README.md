# E-Commerce Sales Optimization  
### Multiple Regression Analysis for Marketing Decision-Making

This project analyzes e-commerce sales performance using multiple regression modeling to identify key drivers of revenue and support data-driven marketing budget allocation decisions.

The analysis is based on a realistic business case involving a large online retailer (“MarketPlace”) and focuses on model building, interpretation, prediction, and strategic insights for executive stakeholders.

---

## Project Overview

**Objective:**  
Build and interpret multiple regression models that explain monthly sales performance and provide actionable insights for marketing and product strategy.

**Key questions addressed:**
- What factors most strongly drive e-commerce sales?
- How effective is digital advertising spend?
- Do seasonality and product categories matter?
- Which regression model is best for prediction and decision-making?
- What are the expected sales for a new product launch?

---

## Dataset

- **File:** `MarketPlace_Sales_Data.csv`
- **Observations:** 3,600 monthly records
- **Time Span:** 18 months
- **Scope:** 200 product subcategories

**Variables include:**
- Sales (response variable)
- Marketing inputs (ad spend, email campaigns, social media engagement)
- Customer behavior (ratings, website traffic)
- Pricing and inventory factors
- Season and product type (categorical variables)

---

## Methodology

This project applies core topics from intermediate and advanced regression analysis, including:

- Dummy variable creation and interpretation  
- Global F-tests and individual t-tests  
- Model selection using Standard Error and Adjusted R²  
- Prediction intervals vs. confidence intervals  
- Partial F-tests for joint significance  
- Coefficient of partial determination  
- Business-focused interpretation of regression outputs  

All analysis is performed in **R** using **R Markdown**.

---

## Key Deliverables

### Problem Statement
The full business case and analytical questions are documented in:  
`problem_statement.md`

---

### Interactive Analysis (HTML)
The best way to explore the complete analysis, including regression outputs, tables, and interpretations.

GitHub Pages link:  
https://ritikagarg0903.github.io/ecommerce-sales-optimization/Ecommerce_Sales_Optimization_RMD.html

---

### Executive Business Report (PDF)
A concise, stakeholder-ready report summarizing key findings, insights, and recommendations.

File:  
`Business_Report.pdf`

---

### Reproducible Analysis Code
The full R Markdown file containing all data preparation, modeling, and analysis steps.

File:  
`Ecommerce_Sales_Optimization.Rmd`

---

## Tools & Technologies

- R / RStudio  
- R Markdown  
- Multiple Linear Regression  
- GitHub Pages  

---

## Key Insights (High Level)

- Digital advertising spend has a statistically significant impact on sales
- Website traffic and customer ratings are strong predictors of revenue
- Seasonality and product type meaningfully influence sales performance
- A simpler regression model performs nearly as well as a full model
- Prediction intervals provide critical guidance for operational planning

Detailed results and interpretations are available in the HTML and PDF reports.

---

## Intended Audience

- Data Analyst and Business Analyst hiring managers
- Business stakeholders interested in data-driven decision-making
- Students reviewing applied regression work

---

## Notes

- Completed as part of an Intermediate Statistics / Regression Analysis course
- AI tools were used only for formatting and writing support, not for analysis
- All interpretations and conclusions are my own