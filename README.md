# Linear Regression – Ames Housing (Zillow Case Study)

## Project Motivation

This project is inspired by Zillow’s **Zestimate** model and the failure of **Zillow Offers** during the COVID-19 pandemic.

Zillow is an online real estate database company that publishes information on over **121 million homes in the U.S.**, collecting data from:

- Public records  
- Owner-submitted data  
- Multiple Listing Services (MLS)  
- Geographic information systems  
- Market trend data  

Zillow’s **Zestimate** is an algorithmic estimate of a home’s market value based on these inputs.

In 2019, Zillow launched **Zillow Offers**, a home-flipping business that:

1. Purchased homes directly from owners  
2. Used algorithmic pricing (Zestimates) to generate offers  
3. Renovated and resold the homes  

However, in **Q3 2021**:
- Zillow lost **$420 million**
- The company shut down Zillow Offers
- CEO Rich Barton stated that Zillow was unable to correctly forecast home prices during the pandemic

---

## What Went Wrong? (Machine Learning Perspective)

The pandemic caused a structural shift in the housing market.

Zillow’s model was trained on pre-pandemic data but deployed in a very different market environment — a classic case of **data drift** (distribution mismatch between training and real-world data).

As a result:
- The model overpaid for homes  
- Market cooling and rising operational costs increased losses  
- Forecast errors amplified business risk  

This project explores similar modeling concepts using the Ames Housing dataset.

---

## Dataset: Ames Housing

This project uses the **Ames Housing Dataset**, which contains residential property sales in Ames, Iowa from **2006–2010**.

### Target Variable
- **Log(Sale Price)**

### Example Features
- Zoning classification  
- Type of dwelling (1-story, 2-story, etc.)  
- Year built  
- Neighborhood  
- Total square footage  
- Lot characteristics  
- Structural and quality features  

---

## Project Objective

Build a **Linear Regression model** to predict log-transformed home prices.

The project demonstrates:

- Data preprocessing  
- Feature handling  
- Train/test split  
- Model fitting using `scikit-learn`  
- Model evaluation  
- Interpretation of regression outputs  
- Discussion of model risk under distribution shift  

---

## Key Concepts Demonstrated

- Ordinary Least Squares (OLS)  
- Bias–variance tradeoff  
- Overfitting  
- Regularization (if implemented)  
- Data drift risk in production systems  
- Limitations of linear models in volatile markets  

---

## Repository Structure
