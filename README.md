# Ecommerce Purchases Dataset Analysis

This project involves the analysis of an Ecommerce Purchases Dataset using Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn. The dataset contains information about purchases made on an ecommerce platform, including details like address, browser information, company, credit card details, and purchase price.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Data Exploration](#data-exploration)

## Project Overview

The goal of this project is to perform data analysis on the Ecommerce Purchases Dataset to extract insights and patterns. The analysis includes checking for null values, identifying the highest and lowest purchase prices, calculating the average purchase price, and more.

## Dataset

The dataset used in this project consists of 10,000 rows and 14 columns. It includes the following columns:
- **Address**: The customer's address.
- **Lot**: The lot number associated with the purchase.
- **AM or PM**: Whether the purchase was made in the AM or PM.
- **Browser Info**: Information about the browser used for the purchase.
- **Company**: The name of the company.
- **Credit Card**: The credit card number used for the purchase.
- **CC Exp Date**: The expiration date of the credit card.
- **CC Security Code**: The security code of the credit card.
- **CC Provider**: The provider of the credit card.
- **Email**: The customer's email address.
- **Job**: The customer's job title.
- **IP Address**: The customer's IP address.
- **Language**: The language used by the customer.
- **Purchase Price**: The purchase price of the item.

## Installation

To run the analysis, you'll need to have Python installed along with the following libraries:
```plaintext
pip install pandas numpy matplotlib seaborn
```
## Usage

To perform the analysis, you can run the Analysis.ipynb notebook, which contains the following steps:

Import Libraries:
```plaintext
import pandas as pd
import numpy as np 
import matplotlib.pyplot as plt 
import seaborn as sns
```
Load the Dataset:
```plaintext
df = pd.read_csv('path_to_your_dataset/Ecommerce Purchases Dataset.csv')
```
Display the Top 10 Rows:
```plaintext
df.head(10)
```
Display the Last 10 Rows:
```plaintext
df.tail(10)
```
Check Data Types of Each Column:
```plaintext
df.dtypes
```
Check for Null Values:
```plaintext
df.isnull().sum()
```
Calculate the Highest and Lowest Purchase Prices:
```plaintext
max_price = df['Purchase Price'].max()

min_price = df['Purchase Price'].min()
```
Calculate the Average Purchase Price:
```plaintext
avg_price = df['Purchase Price'].mean()
```

## Data Exploration

The dataset was explored to uncover various insights, including:

The highest purchase price is 99.99.
The lowest purchase price is 0.00.
The average purchase price is approximately 50.35.
The dataset contains no null values, ensuring data integrity for analysis.
