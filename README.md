# Wine Quality Analysis
This project analyzes the quality of wine based on various chemical properties using a dataset of wine samples. The analysis includes data preprocessing, exploratory data analysis (EDA), model training, and evaluation to predict the quality of wine.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The goal of this project is to predict the quality of wine based on its physicochemical properties. Wine quality is rated on a scale, and the aim is to use machine learning models to determine the quality from the given features.

The dataset used in this project includes attributes like acidity, sugar content, pH, alcohol content, etc. Using these attributes, the project explores various machine learning algorithms to identify the most suitable model for predicting wine quality.

## Dataset
The dataset used for this analysis contains information on wine samples, including:
- **Fixed Acidity**
- **Volatile Acidity**
- **Citric Acid**
- **Residual Sugar**
- **Chlorides**
- **Free Sulfur Dioxide**
- **Total Sulfur Dioxide**
- **Density**
- **pH**
- **Sulphates**
- **Alcohol**
- **Quality** (target variable)

The dataset is sourced from the UCI Machine Learning Repository and is provided in a CSV format ``winequality-white1.csv``.

## Project Structure
The repository is organized as follows:
```
├── Wine quality.ipynb       # Jupyter notebook with the analysis and model training
├── README.md                # Project description and setup instructions
├── data                     # Folder containing the wine dataset
└── models                   # Saved models (if any)
```

## Dependencies
To run the project, you will need the following Python packages:
- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- Jupyter Notebook

You can install the required packages using:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/wine-quality-analysis.git
   cd wine-quality-analysis
   ```

2. Download the dataset and place it in the `data` folder.

3. Open the Jupyter notebook:
   ```bash
   jupyter notebook "Wine quality.ipynb"
   ```

4. Run the cells in the notebook to perform data analysis, train models, and visualize the results.

## Results
### Model Performance
After training multiple models, the following results were obtained:
- **Random Forest Classifier**: Achieved the highest accuracy of approximately 85%, making it the best-performing model for predicting wine quality. This model demonstrated a balanced trade-off between precision and recall.
- **Support Vector Machine (SVM)**: Showed a good accuracy of around 82%, but with higher computational time.
- **Logistic Regression**: Provided an accuracy of 78%, which served as a good baseline for comparison.
  
### Key Insights
- **Alcohol Content**: Higher alcohol levels generally correlated with higher quality ratings.
- **Volatile Acidity**: Wines with lower volatile acidity tended to have better quality ratings.
- **Sulphates and pH**: Sulphate levels had a positive influence on quality, while extreme pH levels negatively impacted the rating.

These insights suggest that certain chemical properties, such as alcohol and acidity, play a significant role in determining the perceived quality of wine.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
