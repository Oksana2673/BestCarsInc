# Vehicles and its Data: An Analysis

## Introduction
First of all, we are going to do an analysis of a database on vehicles. We will use Python libraries such as Pandas, Matplotlib, Seaborn, etc. to interpret multiple aspects of various events, aiming to transform an unreadable database into something much more intelligible.

## Cleaning Data

### Removing Redundant and Sparse Features
- Eliminate redundant or unusable data: Drop the 'URL', 'image_url', and 'city_url' features.
- Dismiss any feature that has over 40% of null values.

_**Question: What are the remaining features?**_

### Removing Outliers
Outlier values are values outside reasonable boundaries. For instance, a sudden 63% drop in Apple stock price may appear to be an outlier. 

We identified an outlier issue with 'price', 'year', and 'odometer':

- Establish a logical range for these three features -- explain your rationale.
- Remove data points (rows) that do not comply with your defined limits.
- Discard any data point with null values.

_**Question: What’s the resulting number of rows? What percentage of rows did we remove due to the cleaning and removing of outliers? Is the dataset still usable? Why?**_


## Feature Relations

- Plot the correlation matrix.
- We observe a positive correlation between price and year. Explain it and code a scatter plot to visualize its relation graphically.
- We also see a negative correlation between price and odometer. Explain it and code a scatter plot.
- Use Seaborn's pairplot() function to analyze all the scatterplots at the same time visually. 

## Feature Analysis

We want to evaluate the distribution of a feature's values:

- Generate a histogram for the 'odometer' feature using 50 bins. You would notice a frequency peak for a specific odometer value range. Explain it.
- Form a histogram for the 'year' feature using 20 bins. A specific year value range will show a frequency highpoint. Explain it.

## Conclusion

Suppose you're the manager of BestCars Inc. Your firm leases all these cars to other companies (like ALD Automotive). However, their storage and upkeep aren't cheap. 

As the boss, you have to make a tough decision:
- Sell all the cars older than a specific year.
- Sell all the cars with significant odometer values (heavy usage).
- Sell all the cars with a bad status (based on the 'condition' feature).

Being an ML Engineer or a Data Scientist is more than just knowing technical aspects. You must also explain what you observe in the data.

_**Reflect: Do I have sufficient data to make a decision? What additional data do I require? Why?**_

## Project Organization
You can document your exercise using markdown or text comments.

## Requirements
You may use any software that supports notebooks, such as VS Code, Jupyter Notebook, Jupyter Lab, Databricks, Google Colab, etc.

## Development
All the development should be conducted using pandas functions in Python (though you're free to use other Python libraries if you wish).

## Resources
- Pandas
- Numpy
- Matplotlib
- Seaborn
