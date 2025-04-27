# Obesity Risk Prediction

This project focuses on predicting obesity levels based on eating habits, physical conditions, and other lifestyle factors. The dataset used for this project is publicly available on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition) under the [CCA 4.0 license](https://creativecommons.org/licenses/by/4.0/legalcode).

## Dataset Overview

The dataset contains 17 attributes and 2,111 samples. These attributes include both categorical and continuous variables, such as:

- **Gender**: Categorical
- **Age**: Continuous
- **Height**: Continuous
- **Weight**: Continuous
- **family_history_with_overweight**: Binary
- **FAVC**: Binary (Do you eat high caloric food frequently?)
- **FCVC**: Integer (Do you usually eat vegetables in your meals?)
- **NCP**: Continuous (How many main meals do you have daily?)
- **CAEC**: Categorical (Do you eat any food between meals?)
- **SMOKE**: Binary (Do you smoke?)
- **CH2O**: Continuous (How much water do you drink daily?)
- **SCC**: Binary (Do you monitor the calories you eat daily?)
- **FAF**: Continuous (How often do you have physical activity?)
- **TUE**: Integer (How much time do you use technological devices?)
- **CALC**: Categorical (How often do you drink alcohol?)
- **MTRANS**: Categorical (Which transportation do you usually use?)
- **NObeyesdad**: Categorical (Target variable - Obesity level)

## Project Workflow

1. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of the target variable.
   - Checked for missing values and summarized the dataset.

2. **Data Preprocessing**:
   - Standardized continuous numerical features using `StandardScaler`.
   - Applied one-hot encoding to categorical features.
   - Encoded the target variable into numerical format.

3. **Model Training and Evaluation**:
   - Implemented multi-class classification using Logistic Regression with:
     - One-vs-All (OvA) strategy.
     - One-vs-One (OvO) strategy.
   - Evaluated the models using accuracy scores.

4. **Experimentation**:
   - Tested the impact of different train-test split ratios on model performance.
   - Analyzed feature importance for both OvA and OvO strategies.

5. **Pipeline Automation**:
   - Developed a reusable function to automate the entire pipeline, from data loading to model evaluation.

## Key Features

- **Multi-class Classification**:
  - Compared One-vs-All and One-vs-One strategies for Logistic Regression.
  - Highlighted the advantages and disadvantages of each approach.

- **Feature Importance**:
  - Visualized the importance of features for both OvA and OvO strategies.

- **Pipeline Automation**:
  - Simplified the process of training and evaluating models with a single function.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/obesity-risk-prediction.git
   cd obesity-risk-prediction
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Obesity_Risk_Prediction.ipynb
   ```

4. Follow the steps in the notebook to explore the dataset, preprocess the data, and train the models.

## Dataset License

The dataset is licensed under the [Creative Commons Attribution 4.0 International License (CCA 4.0)](https://creativecommons.org/licenses/by/4.0/legalcode).

## Acknowledgments

- The dataset is provided by the UCI Machine Learning Repository.
- Special thanks to the contributors of the dataset for making it publicly available.

## Contact

For any questions or suggestions, feel free to reach out at [your-email@example.com].
