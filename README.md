# Insurance All

Insurance All is a company that provides health insurance to its customers and the product team is analyzing the possibility of offering policyholders a new product: A car insurance.

As with health insurance, customers of this new car insurance plan must pay an amount annually to Insurance All in order to obtain an amount insured by the company, destined to the costs of an eventual accident or damage to the vehicle.

Insurance All surveyed nearly 380,000 customers about interest in joining a new auto insurance product last year. All customers showed interest or not in purchasing auto insurance and these responses were saved in a database along with other customer attributes.

The product team selected 127,000 new customers who did not respond to the survey to participate in a campaign, in which they will receive an offer of the new car insurance product. The offer will be made by the sales team through phone calls.

However, the sales team has the capacity to make 20,000 calls within the campaign period.

# 1. Business Problem

1) Main Insights on the most relevant attributes of customers interested in purchasing auto insurance.
2) What percentage of customers interested in purchasing auto insurance will the sales team be able to contact by making 20,000 calls?
3) And if the sales team capacity increases to 40,000 calls, what percentage of customers interested in purchasing auto insurance will the sales team be able to contact?
4) How many calls does the sales team need to make to contact 80% of customers interested in purchasing auto insurance?

## Final Product

- Key insights into customer attributes
- Percentage of interested base customers and whether 20K/40K calls can be met
- Delivery Format Graphics/Table

## Process

- Perform feature engineering in the database of interested customers and raise the hypotheses for each attribute to be validated;
- At EDA, validate hypotheses and identify insights from interested customers;
- Define the delivery format (view, table, sentence)
- Graphics that best demonstrate the information.
- Definition of the storage infrastructure (SQLITE3)
- ETL Design (Extract, Transform and Load Scripts)
- Script scheduling planning (dependency between scripts)
- Define the delivery format (view, table, sentence)
- Perform database analysis and apply ML models to obtain the attributes that define the customer most likely to purchase insurance. With these features define the number of potential customers and whether it is possible to serve with 20/40K calls.

## Enter

Data source:

- Kaggle website
- BD on AWS

Tools:

- Python 3.8.0
- AWS
- Pycharm
- Jupyter Notebook (analysis and prototyping)
- Streamlit

# 2. Data Insights

Below the insights got from the data:

**1. People between 30 years old are more susceptible to have an insurance**- People between 30 years old are more susceptible to have an insurance, 8.09%

**2. Women hire more insurances**- Men hire 3% more insurances than women

**3. Owners with new cars (< 1 yr) hire more insurances**- Owners with cars (> 2 yrs) hire more insurances

**4. People with drive license hire more insurances**- People with a driver's license hire 6.68% more insurance than those without

**5. Owners with vehicle damaged dont hire insurances**- Owners with vehicle damaged hire insurances

**6. People previously insured hire another insurance**- People previously insured hire another insurance

**7. Higher than 50K annual premium there are more insurances**- Higher than 50K annual premium there are more insurances 3.88%


# 3. Machine Learning Model Applied

Below it is listed the ML models applied:
1) KNN
2) Logistic Regresion
3) Extra Trees
4) Random Forest
5) Naive Bayes
6) LGBM
7) XGBoost
8) Guassian NB
9) AdaBoost

# 4. Machine Learning Modelo Performance

| ML Model                | Precision               | Recall             |
|:------------------------|:------------------------|:-------------------|
| KNN                     | 0.3088 +/- 0.0026	      | 0.506 +/- 0.0046   |
| Logistic Regression     | 0.291 +/- 0.0028        | 0.4766 +/- 0.0048  |
| Extra Tress             | 0.313 +/- 0.0036	      | 0.513 +/- 0.0054   | 
| Random Forest           | 0.3186 +/- 0.0039	      | 0.522 +/- 0.0065   |        
| Naives Bayes            | 0.3028 +/- 0.0031	      | 0.496 +/- 0.0048   |
| LGBM                    | 0.3518 +/- 0.0028	      | 0.5762 +/- 0.0047  |
| XGBoost                 | 0.3492 +/- 0.0032	      | 0.5718 +/- 0.0054  |
| Guassian NB             | 0.3028 +/- 0.0031	      | 0.496 +/- 0.0048   |
| AdaBoost                | 0.3336 +/- 0.0016	      | 0.5462 +/- 0.0029  |



