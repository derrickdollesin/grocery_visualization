# The Rise of Highly-Processed Foods: Mapping Food Processing Scores to Price

This project visualizes how grocery stores distribute food items according to processing level and price range. By analyzing grocery store data, we uncover how highly processed foods dominate shelves, especially in the lower price brackets.

## Overview

Using a dataset of food products with attributes such as store, processing score (`FPro_class`), and price, this notebook performs the following:

- Cleans and preprocesses the data
- Bins product prices into labeled ranges (e.g., "$0–10", "$10–20", etc.)
- Maps food processing scores to string labels
- Builds Sankey diagrams using Plotly to illustrate the flow from:
  - Store → Processing Class → Price Bin

Each diagram reveals the structure of food availability at the store level — particularly, how cheaper foods tend to be more processed.

## Tools Used

- Pandas and NumPy for data processing
- Matplotlib and Seaborn for data exploration
- Plotly for building interactive Sankey diagrams
- IPython display utilities to enhance notebook presentation

## Dataset

The dataset (`grocerydb.csv`) includes:
- `store`: store name
- `price`: price of the item
- `FPro_class`: an integer score representing the level of processing

## Running the Notebook

1. Clone the repository
2. Place the `grocerydb.csv` file in a `data/` folder
3. Open and run `final_plot.ipynb` using Jupyter Notebook

```
jupyter notebook final_plot.ipynb
```

## Example Insight

"The cheapest foods at most stores are also the most highly processed. This trend may be contributing to nutritional inequality."
