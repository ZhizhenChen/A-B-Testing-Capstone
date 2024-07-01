# A-B-Testing-Capstone

## Background Introduction
The dataset in this portfolio exercise was originally used as a take-home assignment provided by Starbucks for their job candidates. The data for this exercise consists of about 120,000 data points split in a 2:1 ratio among training and test files. 

In this task, we will use the training data to perform an experiment on starbuck's promotion algorithm, to find out which customers are more likely to be affected by this advertising promotion, and to evaluate if it generated sufficient significance to prove its effective.

## Evaluations
* **Incremental Response Rate (IRR)**

IRR depicts how many more customers purchased the product with the promotion, as compared to if they didn't receive the promotion. Mathematically, it's the ratio of the number of purchasers in the promotion group to the total number of customers in the purchasers group (_treatment_) minus the ratio of the number of purchasers in the non-promotional group to the total number of customers in the non-promotional group (_control_).

$$ IRR = \frac{purch_{treat}}{cust_{treat}} - \frac{purch_{ctrl}}{cust_{ctrl}} $$

* **Net Incremental Revenue (NIR)**

NIR depicts how much is made (or lost) by sending out the promotion. Mathematically, this is 10 times the total number of purchasers that received the promotion minus 0.15 times the number of promotions sent out, minus 10 times the number of purchasers who were not given the promotion.

$$ NIR = (10\cdot purch_{treat} - 0.15 \cdot cust_{treat}) - 10 \cdot purch_{ctrl}$$

## Tasks Description

**Task 1)** 

Check whether the experiment is statistically significant and identify the effect of promotions on indicators.

**Task 2)**

Construct a machine learning model to help detect the user that maximize IRR and NIR.

## Data Description
| # |  Column | Non-Null Count | Dtype |
| --- | --- | --- | --- |
| 0 | ID | 84534 non-null | int64 |
| 1 | Promotion | 84534 non-null | object |
| 2 | purchase | 84534 non-null | int64 |
| 3 | V1 | 84534 non-null | int64 |
| 4 | V2 | 84534 non-null | float64 |
| 5 | V3 | 84534 non-null | float64 |
| 6 | V4 | 84534 non-null | int64 |
| 7 | V5 | 84534 non-null | int64 |
| 8 | V6 | 84534 non-null | int64 |
| 9 | V7 | 84534 non-null | int64 |
