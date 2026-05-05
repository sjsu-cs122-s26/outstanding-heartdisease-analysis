# Indicators of Heart Disease - Data Analysis

## Team Members
- Kyle Arikata
- Brandon Pham
- Brandon Sanchez
- Emily Williams

## Data Set Description
The data set contains survey data from over 400k+ adults in relation to their health status. The data was collected through the CDC and plays a major part in the Behavioral Risk Factor Surveillance System. The data set provides general health indicators as well as an indicator displaying whether or not the respondent has been diagnosed with heart disease.

---
### Dependencies:
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Plotly

---

### Data Setup
 This project uses the **Indicators of Heart Disease (2022 Update)** dataset from Kaggle. Please go to the data directory and follow the README instructions to download the raw dataset. Then upload the file to your Google Drive under `MyDrive/data/`, or update the `file_path` variable in the notebook to match your Drive path.

 ---
 ### How to Run

 #### Google Colab (Recommended)

  1. Open the desired notebook from the `notebooks/` folder directly in Colab (or upload it manually).
  2. When prompted, mount your Google Drive by running the first cell:
  ```python
     from google.colab import drive
     drive.mount('/content/drive')
  ```
  3. Make sure your dataset CSV is placed in the correct Drive path (see Data Setup above).
  4. Run all cells from top to bottom using **Runtime > Run all**.
  
 The notebooks in this project are:
  - `notebooks/main.ipynb` — **Start here.** Performs the initial data exploration and cleaning of the raw dataset (`heart_2022_with_nans.csv`), then exports the cleaned data as `heart_cleaned.csv`. All other notebooks read from this cleaned file.
  - `notebooks/lifestyle_analysis.ipynb` — Behavioral/lifestyle factors and heart disease
  - `notebooks/general_health.ipynb` — General health indicators analysis
  - `notebooks/medical_history.ipynb` — Medical history factors analysis
  - `notebooks/physical_health.ipynb` — Physical health indicators analysis
  
  > **Note:** You must run `main.ipynb` first. It cleans the raw dataset and saves `heart_cleaned.csv`, which is required by all other notebooks.
 
