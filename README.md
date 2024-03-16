# Instacart Market Basket Analysis :shopping_cart:

## Introduction

Instacart is an American technology company that operates as a same-day grocery delivery and pick up service in the U.S. and Canada. Customers shop for groceries through the Instacart mobile app or Instacart.com from various retailer partners. The order is shopped and delivered by an Instacart personal shopper.

### Objectives:
- Analyze the anonymized of 3 million grocery orders from more than 200,000 Instacart users open sourced by Instacart 
- Find out hidden association between products for better cross-selling and upselling
- Perform customer segmentation for targeted marketing and anticipate customer behavior
- Build a Machine Learning model to predict which previously purchased product will be in user’s next order

## Data Overview

[Data](https://www.kaggle.com/c/instacart-market-basket-analysis/data)  is divided across 6 files:

1. **Order Table:**
   - `order_id`: Unique identifier for each order.
   - `user_id`: Unique identifier for each user.
   - `eval_set`: Indicates which evaluation set this order belongs to (train, test, or prior).
   - `order_number`: The sequence number for this order (1 for the first order, 2 for the second, etc.).
   - `order_dow`: The day of the week the order was placed (0 for Sunday, 1 for Monday, etc.).
   - `order_hour_of_day`: The hour of the day the order was placed.
   - `days_since_prior_order`: Days since the last order, capped at 30 (with NAs for order_number = 1).

2. **Products Table:**
   - `product_id`: Unique identifier for each product.
   - `product_name`: Name of the product.
   - `aisle_id`: Identifier for the aisle where the product is located (foreign key).
   - `department_id`: Identifier for the department where the product belongs (foreign key).

3. **Order Products Train Table:**
   - `order_id`: Identifier for the order.
   - `product_id`: Identifier for the product.
   - `add_to_cart_order`: The order in which the product was added to the cart.
   - `reordered`: Indicates if the product was reordered in this order (1 for reordered, 0 otherwise).

4. **Order Products Prior Table:**
   - `order_id`: Identifier for the order.
   - `product_id`: Identifier for the product.
   - `add_to_cart_order`: The order in which the product was added to the cart.
   - `reordered`: Indicates if the product was reordered in this order (1 for reordered, 0 otherwise).

5. **Departments Table:**
   - `department_id`: Identifier for the department.
   - `department`: Name of the department.

6. **Aisles Table:**
   - `aisle_id`: Identifier for the aisle.
   - `aisle`: Name of the aisle.

## Project Organization
```
./
├── EDA
│   └── eda-on-instacart-data.ipynb          
├── Model                                            
│   └── predictive-analysis-model.ipynb 
├── Business Insights 
│   └── Business Questions-Solution.pdf                                              
├── Example of Deployment
│   ├── Instacart Power Bi dashboard.mp4
│   └── Instacart Power Bi dashboard.gif
├── Presentation
│   └── DS - Presentation.pdf 
└── images
```
References:

Instacart: https://www.instacart.com/

