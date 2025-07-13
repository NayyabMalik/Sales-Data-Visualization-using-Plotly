# Sales Data Visualization using Plotly

## Overview

This project, developed as part of the Data Mining course at the National University of Modern Languages, Islamabad, demonstrates data preprocessing and interactive 3D visualization of sales data using Python and Plotly. The project processes a sales dataset with missing values, performs data cleaning, feature engineering, and creates interactive 3D scatter plots to analyze sales metrics (e.g., amount and price) across time dimensions and product categories. It showcases skills in data wrangling, visualization, and interactive dashboard creation, relevant to AI-driven data analysis.

## Dataset

The dataset (`sales_data_missing.csv`) contains sales transactions with the following columns:

- `store_id`: Store identifier
- `customer_id`: Customer identifier
- `product_id`: Product identifier
- `product_category`: Product category (e.g., Toys, Movies, Books)
- `date`: Transaction date and time
- `amount`: Quantity sold
- `single_price`: Price per unit
- `transaction_id`: Unique transaction identifier

The dataset includes missing values in `product_category` and `amount`, which are handled during preprocessing.

## Features

- **Data Preprocessing**:
  - Converts `product_category` to numeric values for analysis.
  - Handles missing values by dropping rows with nulls.
  - Extracts temporal features (year, day, week, quarter, hour) from the `date` column.
  - Drops irrelevant columns (`store_id`, `product_id`, `customer_id`, `transaction_id`).
- **Interactive Visualization**:
  - Uses Plotly to create 3D scatter plots for metrics like amount and price by quarter, day, hour, and week.
  - Implements a Panel-based dashboard with a dropdown menu for selecting different visualizations.
- **Tools and Libraries**:
  - Python: Pandas, NumPy, Plotly, Panel
  - Jupyter Notebook for development and visualization

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/sales-data-visualization.git
   cd sales-data-visualization
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Ensure the dataset (`sales_data_missing.csv`) is in the project directory.

## Usage

1. Open the Jupyter Notebook:

   ```bash
   jupyter notebook Sales_Data_Visualization_using_Plotly.ipynb
   ```
2. Run all cells to preprocess the data and launch the interactive dashboard.
3. Use the dropdown menu in the Panel interface to select different 3D scatter plots (e.g., "Amount by Quarter", "Price by Day").
4. The dashboard will open in a browser at `http://localhost:52383`.

## Repository Structure

```
sales-data-visualization/
├── data/
│   └── sales_data_missing.csv  # Sales dataset
├── Sales_Data_Visualization_using_Plotly.ipynb  # Main notebook
├── requirements.txt  # Python dependencies
├── README.md  # Project documentation
├── LICENSE  # MIT License
```

## Requirements

Install the required libraries using:

```bash
pip install pandas numpy plotly panel
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions, contact \[nayyabm16@gmail.com\] or open an issue on GitHub.