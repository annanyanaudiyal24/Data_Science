**Data Science Assignment 1**

**Overview**

This project performs basic data analysis and data manipulation using Python and Pandas on an International T20 cricket dataset.
The notebook demonstrates common data science operations such as reading data, exploring the dataset, indexing, slicing, and filtering.

**Dataset**

The dataset used in this project is:

**International_T20_Data.csv**

It contains information about international T20 cricket matches including:

- innings information
- match metadata
- match dates
- gender category
- match type

**Technologies Used**

- Python
- Pandas
- Google Colab

**Operations Performed**

**1. Reading the Dataset**

The dataset is loaded using Pandas.

import pandas as pd
df = pd.read_csv('International_T20_Data.csv', engine='python', on_bad_lines='skip')

**2. Dataset Exploration**

Basic exploration of the dataset.

df.shape
df.head()
df.tail()
df.describe()

**3. Indexing and Slicing**

Selecting rows and columns using Pandas indexing.

df.iloc[:, -3:]
df.loc[50:60, ['innings', 'meta.data_version', 'meta.created']]
df[0:20]

**4. Column Selection**

Selecting specific columns from the dataset.

df[['info.dates', 'info.gender', 'info.match_type']]

**5. Boolean Indexing**

Filtering data using conditions.

df['info.dates'] == 'en'
gender = df[df['info.gender'] == 'en']
gender.head()

**Objective**

The goal of this assignment is to understand:

- Data loading
- Data exploration
- Indexing and slicing
- Column selection
- Boolean filtering using Pandas

**Author**

Annanya Naudiyal

**Environment**

This project was developed and executed using Google Colab.
