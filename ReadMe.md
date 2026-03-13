
# Telecom Customer Churn Analysis

## Project Overview

Customer churn is a major challenge in the telecommunications industry, as acquiring new customers is significantly more expensive than retaining existing ones. Understanding the factors that contribute to churn can help companies develop targeted retention strategies and improve long-term profitability.

This project explores a telecommunications customer dataset to identify patterns and key drivers of churn. Using **data cleaning, exploratory data analysis (EDA), and data visualisation**, the analysis aims to uncover insights into customer behaviour and highlight potential strategies to reduce churn.

---

# Objectives

The main objectives of this project are to:

* Analyse customer data to understand patterns related to churn.
* Identify key factors that influence whether a customer leaves the company.
* Explore how **contracts, services, and billing structures** affect churn rates.
* Provide **data-driven insights and recommendations** that could help improve customer retention.
* Visualize customer behavior through an **interactive Tableau dashboard**.

---

# Dataset

The dataset used in this project is adapted from the **IBM Telco Customer Churn dataset**, which is commonly used for data science and analytics practice.

### Dataset Size

* **Rows:** 7,043 customers
* **Columns:** 21 features

### Key Variables

| Feature                       | Description                                               |
| ----------------------------- | --------------------------------------------------------- |
| CustomerID                    | Unique customer identifier                                |
| Gender                        | Male or Female                                            |
| SeniorCitizen                 | Indicates whether the customer is a senior citizen        |
| Partner                       | Whether the customer has a partner                        |
| Dependents                    | Whether the customer has dependents                       |
| Tenure                        | Number of months the customer has stayed with the company |
| PhoneService                  | Whether the customer has phone service                    |
| InternetService               | Type of internet service (DSL, Fiber optic, None)         |
| TechSupport                   | Whether the customer has technical support                |
| OnlineSecurity                | Whether the customer has online security services         |
| StreamingTV / StreamingMovies | Entertainment services                                    |
| Contract                      | Contract type (Month-to-month, One year, Two year)        |
| MonthlyCharges                | Monthly bill amount                                       |
| TotalCharges                  | Total amount charged to the customer                      |
| Churn                         | Indicates whether the customer left the company           |

---

# Data Cleaning

Before conducting the analysis, the dataset was cleaned to ensure accuracy and consistency.

Steps included:

* Converting the **TotalCharges column to numeric format**
* Handling missing values
* Creating a **binary churn variable** for analysis
* Preparing features for visualisation and aggregation

---

# Exploratory Data Analysis

Several analyses were conducted to understand the factors associated with churn.

## Churn Overview

* Total customers: **7,043**
* Customers who churned: **1,869**
* Overall churn rate: **26.5%**

This indicates that approximately **one in four customers leave the company**, highlighting the importance of retention strategies.

---

## Contract Type and Churn

Contract length has a strong relationship with churn:

| Contract Type  | Churn Rate |
| -------------- | ---------- |
| Month-to-month | 42.7%      |
| One-year       | 11.3%      |
| Two-year       | 2.8%       |

Customers on **month-to-month contracts are significantly more likely to churn**, while long-term contracts show much stronger retention.

---

## Revenue and Charges

### Monthly Charges

Customers with higher monthly bills tend to have **higher churn rates**, suggesting that price sensitivity may influence customer decisions.

### Total Charges

Customers with **low total charges (<500)** show the highest churn rates, which suggests that **new customers are more likely to leave early**.

Long-term customers with higher lifetime spending show **much lower churn rates**.

---

## Services and Customer Behaviour

Service subscriptions also influence churn patterns.

### Internet Service

| Internet Service | Churn Rate |
| ---------------- | ---------- |
| Fiber Optic      | 41.9%      |
| DSL              | 18.9%      |
| No Internet      | 7.4%       |

Fiber optic users show the **highest churn**, possibly due to higher costs or service expectations.

---

### Technical Support

| Tech Support | Churn Rate |
| ------------ | ---------- |
| No           | 41.6%      |
| Yes          | 15.2%      |

Customers without tech support churn **almost three times more frequently**, indicating that support services improve retention.

---

### Online Security

| Online Security | Churn Rate |
| --------------- | ---------- |
| No              | 41.8%      |
| Yes             | 14.6%      |

Security services appear to significantly **reduce churn risk**.

---

### Streaming Services

Streaming services show a weaker relationship with churn, suggesting that entertainment features alone do not strongly influence retention.

---

# Key Insights

The analysis reveals several important patterns:

* **Contract length is one of the strongest predictors of churn.**
* **New customers are more likely to leave early in their lifecycle.**
* **Fiber optic customers represent the highest-risk segment.**
* **Value-added services such as Tech Support and Online Security significantly reduce churn.**

These insights suggest that improving customer support and encouraging longer contracts could reduce churn.

---

# Tableau Dashboard

An interactive Tableau dashboard was created to visualise churn patterns across contracts, services, and customer segments.

The dashboard allows users to explore:

* Overall churn trends
* Churn by contract type
* Churn by services and subscriptions
* Revenue-related churn patterns

---

# Tools and Technologies

This project was developed using the following tools:

* **Python**
* **Pandas**
* **NumPy**
* **Jupyter Notebook**
* **Tableau**
* **GitHub**

---

# Future Work

Possible extensions of this project include:

* Building **machine learning models to predict churn**
* Developing **customer risk scoring systems**
* Identifying **high-risk customer segments for targeted retention strategies**
