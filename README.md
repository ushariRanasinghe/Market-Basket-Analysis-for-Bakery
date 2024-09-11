# Market Basket Analysis

## Overview

This project performs Market Basket Analysis on transaction data to uncover purchasing patterns and relationships between products. By leveraging association rule mining techniques, such as the Apriori algorithm, the analysis identifies frequently bought itemsets and generates insightful association rules. Data visualization is achieved through various plots and interactive network graphs.

## Introduction to Apriori Algorithm

The Apriori algorithm is a classic algorithm used in data mining for association rule learning. It identifies frequent itemsets in transaction data and generates association rules to uncover patterns in purchases. The algorithm operates on the principle that if an itemset is frequent, all of its subsets must also be frequent. This approach iteratively prunes infrequent itemsets and builds up the frequent itemsets, which are then used to generate association rules. These rules help in understanding relationships between items, such as "if a customer buys bread, they are likely to buy butter."

## Features

- **Data Exploration**: Provides insights into transaction frequencies, item counts, and time-based patterns.
- **Association Rule Mining**: Uses the Apriori algorithm to discover frequent itemsets and generate association rules.
- **Interactive Visualizations**: Utilizes Plotly to create interactive network graphs of item associations and seaborn/matplotlib for detailed plots.

## Installation

Ensure you have the following packages installed:

- pandas
- numpy
- matplotlib
- seaborn
- mlxtend
- networkx
- plotly

You can install them via pip:

```bash
pip install pandas numpy matplotlib seaborn mlxtend networkx plotly
```

## Usage

1. **Load Data**:
   ```python
   import pandas as pd

   df_up = pd.read_csv('../input/the-bread-basket/bread basket.csv')
   ```

2. **Data Exploration**:
   - Explore dimensions, null values, and duplicates.
   - Analyze transaction counts by time periods and plot visualizations.

3. **Transaction Categorization**:
   - Define periods of the day and categorize transactions based on item combinations.
   - Generate and display pie charts of transaction distributions.

4. **Association Rule Mining**:
   - Apply the Apriori algorithm to identify frequent itemsets and generate association rules.
   - Visualize the relationships between items using interactive network graphs.

5. **Visualize Results**:
   - Generate bar plots for transaction counts by hour and item frequency.
   - Create pie charts for transaction distribution by item category.
   - Plot interactive network graphs to visualize item connections using Plotly.

