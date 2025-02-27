# Edge_Project


## Overview
This project is a Kaggle dataset analysis using Google Colab. It includes data extraction, preprocessing, and analysis.

## Dependencies

This project requires the following libraries:

- `numpy`
- `pandas`
- `scikit-learn`
- `zipfile`
- `google.colab` 

## Setup Instructions
1. **Mount Google Drive**
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
2. **Extract Dataset** (if zipped)
   ```python
   import zipfile
   with zipfile.ZipFile('/content/drive/MyDrive/archive(kk).zip', 'r') as zip_ref:
       zip_ref.extractall('/content/drive/MyDrive/kaggle_project')
   ```
3. **Load Dataset**
   ```python
   import pandas as pd
   df = pd.read_csv("/content/drive/MyDrive/kaggle_project/timesData.csv")
   ```

## Data Preprocessing
- Dropping unnecessary columns:
  ```python
  df.drop('university_name', axis=1, inplace=True)
  ```


## Usage

1. Load the dataset (either from Kaggle or Google Drive).
2. Perform data preprocessing, including missing value imputation and feature encoding.
3. Apply machine learning models (e.g., Linear Regression) for predictions.
4. Evaluate model performance using relevant metrics.



## File Structure

- `kaggle_project.ipynb`: Notebook containing data processing and model training steps.

## Contributing

Feel free to fork and modify the notebook for further analysis. Contributions are welcome!

## License

This project is for educational purposes and follows an open-source license.


