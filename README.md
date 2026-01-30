Exoplanet Detection from Kepler Space Telescope Data

1. Project Overview

This project aims to identify exoplanets using the Transit Method. When a planet passes in front of its host star, it causes a tiny, periodic dip in the star's brightness.

The primary challenge of this dataset is the extreme class imbalance: out of thousands of stars, only a handful harbor confirmed exoplanets. Our solution focuses on maximizing Recall, ensuring that no potential discovery is missed by the automated system.

2. Key Features

Feature Engineering: Uses Fast Fourier Transform (FFT) to convert light intensity from the Time Domain to the Frequency Domain, revealing hidden orbital rhythms.

Advanced Statistical Extractors: Calculates skewness, kurtosis, and signal-to-noise ratios to distinguish between cosmic noise and real transits.

Ensemble Modeling: Combines Random Forest and cost-sensitive XGBoost models to handle the 1:100 class imbalance.

Astronomical Impact: Achieves 100% Recall on the test set, reducing the manual verification workload for astronomers by over 90%.

3. Repository Structure

EXOPLANET_MODEL_FINAAAL.ipynb: The complete project notebook including data cleaning, EDA, modeling, and results interpretation.

requirements.txt: List of Python libraries required to reproduce the results.

4. How to Use

Clone the repository:

git clone [https://github.com/LALLEARABY/Exoplanet-Detection-Project.git](https://github.com/LALLEARABY/Exoplanet-Detection-Project.git)


Install dependencies:

pip install -r requirements.txt


Run the Notebook: Open the .ipynb file in Google Colab or Jupyter Lab. Ensure you have the exoTrain.csv and exoTest.csv files available in your working directory.

5. Dataset

The data used in this project is sourced from NASA's Kepler mission.
[[kepler-labelled-time-series-data](https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data)]

Author: [LALLE BABA ARABIE]
Date: January 2026
