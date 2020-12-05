# Lending Club

Lending Club is a US peer-to-peer lending company, headquartered in San Francisco, California. Lending Club enables borrowers to create unsecured personal loans between $1,000 and $40,000. The standard loan period is three years. Investors can search and browse the loan listings on Lending Club website and select loans that they want to invest in based on the information supplied about the borrower, amount of loan, loan grade, and loan purpose. Investors make money from interest. Lending Club makes money by charging borrowers an origination fee and investors a service fee. Lending Club enables borrowers to create loan listings on its website by supplying details about themselves and the loans that they would like to request. All loans are unsecured personal loans and can be between $1,000 - $40,000. On the basis of the borrower’s credit score, credit history, desired loan amount and the borrower’s debt-to-income ratio, Lending Club determines whether the borrower is credit worthy and assigns to its approved loans a credit grade that determines payable interest rate and fees. 



My client was related to Good Credit Score and I had to analyze and provide insights related to his credit history and predict the future behavior for the lending club.



## Codelabs 

https://codelabs-preview.appspot.com/?file_id=12ss14yJIFXXGqc5jvIBk3HMztAAI9UywW7h9zYXB7TU#0



## Getting Started

The steps required to install and deploy the project in live system are as follows:

### Prerequisites 

To begin with I need to install python 2.x/3.x in our local system and add it to our classpath. Some python packages are also needed for deployment

```
Python packages:

auto-sklearn
h2o
tpot
featuretools
seaborn
matplotlib
```

Installing

Following steps are required to install necessary packages

Install python packages mentioned above using pip command

```
pip install requirements.txt
```



**Feature Engineering**

Feature engineering is the process of taking a dataset and constructing explanatory variables  and  features ,  that can be used to train a machine learning model for a prediction problem. Often, data is spread across multiple tables and must be gathered into a single table with rows containing the observations and features in the columns.

I performed 2 types of feature engineering

a. Manual Feature Engineering

b. Automated Feature Engineering using Featuretools

**Manual Feature Engineering**

The traditional approach to feature engineering is to build features one at a time using domain knowledge, a tedious, time-consuming, and error-prone process known as manual feature engineering. The code for manual feature engineering is problem-dependent.



**Automated Feature Engineering**

Automated feature engineering allows even a domain novice such as myself to create thousands of relevant features from a set of related data tables. All I need to know is the basic structure of our tables and the relationships between them which I track in a single data structure called an entity set. Once I have an entity set, using a method called Deep Feature Synthesis (DFS), I was  able to build thousands of features in one function call.



**Prediction**

Built 3 models with Linear Regression,Random Forest,Neural Networks Model.Calculated MAPe for all three models and chose the best model.

Also performed 5 fold cross  validation across all the three models.

*HyperParameter Tuning*

For each model tuned different parameters like

a. Regression: Try L1, L2, Elasticnet regularization
b. Neural networks: Change epochs, optimizers, learning rate
c. Random forest: No of trees, Tree depth

**AutoML**

Used three open source tools to calculate MAPe for each model.The three tools are;

a. TPOT
b. AutoSKLearn
c. H2o.ai



**Analysis**

Built several test cases related to the good credit client and specified features which would help him benefit from the lending club.




## Built With

* [Jupyter Notebook](https://jupyter-notebook.readthedocs.io/en/stable/) - Code editor used for python
