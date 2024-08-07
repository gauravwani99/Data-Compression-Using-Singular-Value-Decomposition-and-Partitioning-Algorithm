# README

This repository contains Python scripts for processing and analyzing multiple CSV files related to power system data. The scripts perform various tasks such as data preprocessing, visualization, dimensionality reduction, compression using singular value decomposition (SVD), and evaluation of compression results.

## Prerequisites
- Python 3.x
- Required Python packages: `numpy`, `pandas`, `matplotlib`

## Usage
- Make sure the required Python packages are installed.
- Place the CSV files in the same directory as the scripts.
- Run the appropriate script for the desired set of CSV files.

## Files
- `Ang_Freq_Fault.csv`
- `Frequency_Load_Outage.csv`
- `Vang_Fault.csv`
- `Vang_Load_Outage.csv`
- `Vmag_Fault.csv`
- `Vmag_Load_Outage.csv`
- `Book3.csv`
- `README.md`: This file

## Scripts
### SVD_final_code1.py
- Processes the first six CSV files: `Ang_Freq_Fault.csv`, `Frequency_Load_Outage.csv`, `Vang_Fault.csv`, `Vang_Load_Outage.csv`, `Vmag_Fault.csv`, `Vmag_Load_Outage.csv`.
- Performs data preprocessing including dropping the 'Time' column.
- Applies dimensionality reduction and compression using SVD.
- Evaluates compression performance.

### SVD_final_code2.py
- Processes the last CSV file: `Book3.csv`.
- Performs data preprocessing including dropping the last row and columns ["Unnamed: 10", "Unnamed: 11", "Unnamed: 12", "Unnamed: 13", "Unnamed: 14", "Domain"].
- Applies dimensionality reduction and compression using SVD.
- Evaluates compression performance.

## Output
- Visualization of original data (if applicable).
- Compression ratio, RMSE error, and MADE error at each compression step.
- Plot of columns of the reconstructed matrix (if applicable).
- Plot of estimated rank vs. timestamp (if applicable).
- Comparison of original and reconstructed data (if applicable).

## Additional Notes
- Ensure that the CSV files contain data in the expected format for proper execution of the scripts.
- Adjust parameters like target SNR, sampling rate, and compression parameters as needed.
- The scripts provide insights into data compression and error estimation for power system data analysis.
