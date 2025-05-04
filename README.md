# Flood Claims Forecasting with ONI using SARIMAX

This project combines U.S. flood insurance claims, population estimates, and climate data (ONI) to build predictive models for flood risk forecasting in Texas. The pipeline includes data preparation, dataset merging, and time series model execution using SARIMAX.

---

## 📥 Step 1: Import FEMA Claims Data

1. Download the **NFIP Claims Dataset** (CSV) from FEMA.  
   🔗 [https://www.fema.gov/openfema-data-page/fima-nfip-redacted-claims-v2](https://www.fema.gov/openfema-data-page/fima-nfip-redacted-claims-v2)

2. Follow instructions in the `import/README.md` file to prepare the dataset.

3. **Place the downloaded file in the `import/` directory** of this repository.

---

## 🔄 Step 2: Run Data Management Notebooks

1. Clone or navigate to the data management repo:  
   🔗 [https://github.com/hirokoclanger/floods/tree/main/code/data-management](https://github.com/hirokoclanger/floods/tree/main/code/data-management)

2. Open and run the following Jupyter Notebooks in order:
   - `1_fetchData.ipynb` – loads and pre-processes FEMA and NOAA datasets.
   - `2_mergeDataSets.ipynb` – aligns claims, population, and ONI datasets into a single time series.

---

## 🔍 Step 3: Run Modeling Notebooks

After merging the data, proceed to the modeling phase:

1. Navigate to the `models/` directory.

2. Run the modeling notebooks:
   - `SARIMAX.ipynb` – builds SARIMAX model with ONI as an exogenous regressor.
   - `ARIMA.ipynb` – builds ARIMA.

---

## 🗂 Directory Structure Overview