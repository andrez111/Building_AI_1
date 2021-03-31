# Building_AI_1
Draft project for Reaktor - Building AI Course

# Project Title

Non-Performing Loans Predictor

## Summary

Our Algorithm aims to predict the status of existing credit lines, giving back the probability that credit will become NPL. This can give to financial institutions and citizens the possibility to avoid risks.

## Background

NPLs are the most poisoning and dangerous category of assets in the financial system. Their low probability of repayment affects the balance sheet of banks, posing at risk their ability to fully function as financial lenders.

* Problem: Avoid NPLs by assign them a probabilty of default.
* Frequency: in the EU Zone, up to 2019, there are more than 600 Billion of NPLs
* Motivation: Italian credit system is under pressure due to the massive presence of NPLs in Banks balance sheets. This led to a constant credit shortage on the retail market and higher intrest rates for borrowers.

## How is it used?

PROCESS:
   * Define the financial variables that are used to reach the classification of NPL.
   * Define the dataset of publicly available information that can populate the model (training, test and dev data)
   * Set the tolerance in order to tag the acceptable risk level.

<img src=https://github.com/andrez111/Building_AI_1/blob/main/Building%20AI%201.png>

 Describe the process of using the solution. In what kind situations is the solution needed (environment, time, etc.)? Who are the users, what kinds of needs should be taken into account?

* Step 1: extract anonymized credit data from public databases.
                                                               
* Step 2: Define the set of variables to be analyzed: 
  > A) past credit history
  > B) number of financing events in life 
  > C) payment score: sum of days of overdue

* Step 3: Apply a Naive Bayes classifier to filter over a set confidence level each variable.

* Step 4: If the variable is accepted, we can use it within a linear regression model setting up relative weights.

The model can be used during credit evaluation performed by banks and financial professioanls, both with individuals and corporations. 
We should take into account the availabilty of fresh data, and the fact that the purchasing power can change over time.


## Data sources and AI methods
Where does your data come from? Do you collect it yourself or do you use data collected by someone else?
If you need to use links, here's an example:
[Crif API](https://www.crif.it/consumatori/il-sistema-di-informazioni-creditizie/)
[Banca D'Italia](https://arteweb.bancaditalia.it/arteweb-fe-web/cr)

| Syntax      | Description |
| ----------- | ----------- |
| Naive Bayes Class   |  A) |
| Naive Bayes Class   |  B) |
| Naive Bayes Class   |  C) |

Linear regression model = Weighted (A + B + C)

## Challenges

WE must consider that past history cannot be always a good way to predict the future. From an ethical point of view: if we reduce the impact, on one side, of the NPL problem, on the other side we create a system that can eventually exclude some categories to access credit.

## What's next?

CODING; CODING and CODING. With a set of skills useful to define the input of the model. 
We can assume that this NPL prediction model can firstly reduce the risk of contagion within the credit system, and then to create specific instruments to fulfil the needs of least powerful people that have to access credit to change their status.

## Acknowledgments

I didn't find the company that I loved to work within, so I create it.
