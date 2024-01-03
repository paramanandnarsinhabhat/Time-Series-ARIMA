
# Time-Series Analysis with ARIMA

This project focuses on applying the Autoregressive Integrated Moving Average (ARIMA) model to analyze and forecast time-series data. It includes preprocessing steps, stationarity checks, and the use of Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) plots to determine the ARIMA model parameters.

## Project Structure

```
TIME-SERIES-ARIMA
│   .gitignore
│   requirements.txt    
│
├── data
│   ├── train
│   │   └── train_data.csv
│   └── valid
│       └── valid_data.csv
│
├── myenv                   # Virtual environment directory
│
├── notebook                # Jupyter notebooks for analysis
│   └── ACF and PACF.ipynb
│
└── scripts                 # Python scripts for ARIMA modeling
    └── train_series_arima.py
```

## Installation

To set up the project environment, follow these steps:

1. **Clone the repository** to your local machine.

2. **Create and activate a virtual environment** (recommended):

```bash
python -m venv myenv
source myenv/bin/activate  # On macOS and Linux
myenv\Scripts\activate     # On Windows
```

3. **Install the required packages** listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

## Workflow

- Load the training and validation data from the CSV files in the `data` directory.
- Convert the date columns to datetime objects for time-series analysis.
- Plot the training and validation data to visualize the time-series.
- Conduct Dickey-Fuller and KPSS tests to assess the stationarity of the series.
- Transform the series to achieve stationarity through differencing and logarithmic transformation.
- Use ACF and PACF plots to determine the ARIMA model parameters.
- Run the ARIMA model using the identified parameters.

## Usage

- Execute the script to train the ARIMA model:

```bash
python scripts/train_series_arima.py
```

- Alternatively, open and run the Jupyter notebook for an interactive session:

```bash
jupyter notebook notebook/ACF and PACF.ipynb
```

## Contributing

Contributions to this project are welcome. Please feel free to fork the repository, make changes, and submit pull requests.

## License

This project is licensed under the MIT License.
```
