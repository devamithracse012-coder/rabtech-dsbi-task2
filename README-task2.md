# RabTech Task 2 — Data Ingestion, Cleaning & Preprocessing

## Files
- `Data_Cleaning_Preprocessing.ipynb` — executable Pandas notebook
- `retail_store_sales.csv` — raw 12,575-row dataset
- `clean_dataset.csv` — standardized output produced by the notebook

## How to run
1. Keep all three files in the same folder.
2. Open the notebook in Jupyter Notebook/JupyterLab.
3. Run all cells from top to bottom.
4. The final cell exports `clean_dataset.csv`.

## Cleaning performed
- Corrected dates and numeric data types
- Removed exact duplicate records
- Handled missing categorical values
- Imputed missing numeric values using category medians
- Reconstructed missing total spend from price × quantity
- Detected and capped IQR-based numeric outliers while retaining audit flags
- Extracted Year, Month and Month_Name
- Created Revenue

## Profit-margin note
The source dataset does **not** contain actual cost/profit data. To demonstrate the requested margin feature without hiding the limitation, the notebook uses an **illustrative 70% cost-rate assumption** and names the resulting fields `Estimated_Cost`, `Estimated_Profit`, and `Estimated_Profit_Margin`. These are not accounting figures.
