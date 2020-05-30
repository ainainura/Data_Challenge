# Data Challenge

Two different datasets are given to be analyzed - IRS public dataset and US Census dataset. 

## Goal

The goal here is to explore both datasets, find interesting trends, and create some cohesive stories. Data visualization is used in order to support results and conclusions. 

Description of the datasets: 

## irs_public_data.csv:

This data is public data released by the IRS about personal income taxes filed during the 2013 tax year.
 
The columns are defined here:

STATE: 2 letter state abbreviation.

zipcode: 5 digit ZIP code. If this is 0, the row refers to the whole state.

agi_stub: A categorical of 1-6, indicating the "adjusted gross income" bracket represented by the row: 
    1 = $1 under $25,000
    2 = $25,000 under $50,000
    3 = $50,000 under $75,000
    4 = $75,000 under $100,000
    5 = $100,000 under $200,000
    6 = $200,000 or more
    
num_returns: The total number of returns represented by this row.

num_single_returns: Total number of returns with a filing status of "single."

num_joint_returns: Total number of returns with a filing status of "married, filing jointly."

num_head_of_household_returns: Total number of returns with a filing status of "head of household."

num_paid_preparer_returns: Total number of returns with a paid preparer's signature.
    Returns prepared by tax stores and accountants have paid preparer's signatures.
    Returns prepared by hand or by tax software do not have paid preparer's signatures.
    
num_exemptions: Summed total number of exemptions claimed on form 1040, line 6D.

num_dependents: Summed total number of dependents claimed on forms 1040, line 6C.

amount_agi: Summed total adjusted gross income claimed on forms 1040, line 37; 1040A, line 21; 1040EZ line 4.

num_returns_with_refunds: Total number of returns that claim refunds of overpayment on forms 1040, line 73; 1040A, line 42; 1040EZ, line 11A.

amount_refunds: Summed total amount of overpayments refunded.

## acs_population_demographics.csv

This is a simplified dataset released by the American Community Survey (part of the US Census) showing detailed estimates of the age and sex breakdown of the population by ZCTA (ZIP code tabulation area), a rough equivalent of zip code.

Unless the column is titled "Total," the population estimates are percentages.
