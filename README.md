# anticipating-the-next-pitch

## Overview
This project provides a classification model approach to predicting the next pitch in a plate appearance during MLB games using only prior-pitch features.

## Table of Contents
- [Overview](#overview)
- [Data](#data)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Data
The final dataset merges three queries all from Statcast (PyBaseball)
1. 2024 pitch-by-pitch data from all games ranging from April to September
2. 2023 aggregated pitch distributions by pitcher
3. 2023 aggregated pitch distributions by hitter


## Project Structure
```
.
├── data/
│   └── cached_pitcher_statcast.csv
├── project.ipynb
├── README.md
├── requirements.txt
```

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/Joshua-Wehner/anticipating-the-next-pitch.git
   ```
2. Install dependencies (Python 3.8+ recommended):
   ```sh
   pip install -r requirements.txt
   ```
   Or manually install:
   ```sh
   pip install pandas numpy matplotlib seaborn scikit-learn pybaseball joblib
   ```

## Usage
Open `modeling.ipynb` in Jupyter or VS Code and run the cells sequentially. The notebook covers:
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- PCA Analysis
- Classification Modeling (Logistic, Decision Tree, Random Forest, Adaboost, K-nearest Neighbor, Neural Network)

## Results
- Clustering on pitch type.
- Cross-validated modeling developed and compared.
- See notebook for plots and detailed findings.

## License
MIT License.

