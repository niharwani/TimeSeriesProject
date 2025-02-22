# Time Series Data Visualization Using Python

## Project Overview

This project focuses on visualizing and analyzing time series data using Python. By leveraging libraries such as `pandas`, `matplotlib`, `seaborn`, and `statsmodels`, the project demonstrates techniques for data loading, preprocessing, visualization, and decomposition to extract meaningful insights from temporal datasets.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Dataset Description](#dataset-description)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)

## Installation

To replicate this project, ensure you have Python installed on your system. Follow the steps below to set up the necessary environment:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/niharwani/TimeSeriesProject.git
   cd TimeSeriesDataVisualization
   ```

2. **Create a Virtual Environment:**

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment:**

   - On Windows:

     ```bash
     venv\Scripts\activate
     ```

   - On macOS and Linux:

     ```bash
     source venv/bin/activate
     ```

4. **Install Required Libraries:**

   ```bash
   pip install -r requirements.txt
   ```

## Dataset Description

The project utilizes a time series dataset stored in `stock_data.csv`. The dataset should contain at least two columns:

- `Date`: The date or timestamp of the observation.
- `Value`: The numerical value corresponding to the date.

**Sample Structure:**

| Date       | Value |
|------------|-------|
| 2025-01-01 | 123   |
| 2025-01-02 | 150   |
| 2025-01-03 | 98    |
| ...        | ...   |

*Ensure that the 'Date' column is in a recognizable date format.*

## Usage

Follow the steps below to run the time series visualization script:

1. **Place the Dataset:**

   Ensure `data.csv` is located in the project directory.

2. **Run the Script:**

   Execute the Python script to generate visualizations:

   ```bash
   python time_series_visualization.py
   ```

   The script will perform the following:

   - Load and preprocess the data.
   - Plot the original time series.
   - Decompose the series into trend, seasonal, and residual components.
   - Display the resulting plots for analysis.

## Visualizations
Here are the key visualizations used in the analysis:

1. **ACF Plot** (`acf_plot.png`)
   - Displays the autocorrelation function (ACF) of the time series to identify seasonal and lag-based patterns.

2. **Original vs Differenced Time Series** (`original_vs_differenced_high.png`)
   - Compares the original time series with its differenced version to remove trends and make it stationary.

3. **Original vs Moving Average (120-Window)** (`original_vs_moving_avg_120.png`)
   - Shows the original time series alongside a moving average with a window of 120, highlighting long-term trends.

4. **Monthly Resampling - Highest Price** (`monthly_resampling_highest_price.png`)
   - Aggregates the data at a monthly level and plots the highest price observed in each month.


## Contributing

Contributions are welcome! If you'd like to enhance this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## Acknowledgments

- [pandas](https://pandas.pydata.org/)
- [matplotlib](https://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
- [statsmodels](https://www.statsmodels.org/)

*Inspired by tutorials and resources from the data science community.*

---

*This README template is adapted to provide a comprehensive overview of the Time Series Data Visualization project, ensuring clarity and ease of replication.* 
