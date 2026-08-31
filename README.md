# House Price Prediction

A machine-learning project that predicts residential property prices from structured housing data. The project includes exploratory data analysis, data preparation, model training, evaluation, and a notebook section for generating manual predictions from user-entered property features.

## Overview

This project uses Python and Jupyter Notebook to build and evaluate a house-price prediction workflow. The notebook prepares the dataset, splits records into training and test sets, compares predictive models, evaluates model performance, and allows a user to enter property values to generate a price prediction.
!!Important: The current model is limited by the features available in the dataset. Its predictions use only the included property attributes.

## Features

- Data loading and exploratory analysis
- Data cleaning and preprocessing
- Training/test data splitting
- Machine-learning model training and comparison
- Model evaluation using test data
- Random sampling of test-set records for manual prediction experiments
- Manual property-feature input for individual price predictions

## Technologies

- Python
- Jupyter Notebook
- Miniconda / Conda
- pandas
- NumPy
- scikit-learn
- Matplotlib and Seaborn

## Installation

### Prerequisites

- Windows, macOS, or Linux
- [Miniconda](https://www.anaconda.com/download/)
- Git is optional if you download the project as a ZIP file instead of cloning it

This repository includes an `environment.yml` file that defines the Python version and packages required for the project.

### Option 2: Download ZIP

1. Select **Code → Download ZIP** from the GitHub repository page.
2. Extract the downloaded ZIP file to a location of your choice.
3. Open Anaconda Prompt on Windows, or a terminal on macOS/Linux.
4. Navigate to the extracted project folder.

For example, on Windows:

```bat
cd "C:\path\to\HousePricePrediction"
```

Use the following commands when needed:

```bat
dir
cd folder-name
```

## Create the Conda Environment

From the project directory that contains `environment.yml`, run:

```bash
conda env create -f environment.yml
```

This creates the Conda environment and installs the dependencies specified in the environment file.

Then activate the environment:

```bash
conda activate HousePricePrediction
```

> If your `environment.yml` uses a different environment name, use that exact name instead.

## Run the Notebook

With the Conda environment activated, start Jupyter Notebook:

```bash
jupyter notebook
```

Jupyter should open in your default browser. In the Jupyter file browser:

1. Open `HousePricePrediction.ipynb`.
2. In the notebook menu, select **Run → Run All Cells**.
3. Review the data-preparation, model-training, and evaluation output.

## Manual Predictions

The notebook includes a section for entering property values and generating an individual price prediction.

1. Find the notebook section labeled `6.2`.
2. Run the cell above the manual-input cell to display five randomly selected records from the test set.
3. Use one of those records as a reference when entering sample feature values.
4. Find the cell marked with a comment similar to:

```python
# Modify these values to get manual predictions.
```

5. Update the feature values in that cell.
6. Run the cell to generate a predicted house price.

You can rerun the test-set sample cell to display a different set of five example records.

## Future Improvements

- Add a Streamlit or Flask interface for interactive predictions
- Add automated tests for data-preprocessing functions
- Add model-performance charts and comparison tables to the README
- Package preprocessing and prediction code into reusable Python modules
- Add model versioning and experiment tracking
- Automatic model tuning

## Author

Jair Palacios
