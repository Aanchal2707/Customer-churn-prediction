# Customer Churn Prediction

This repository contains a machine learning project focused on predicting customer churn. The project includes data preprocessing, visualization, feature extraction, model training, and evaluation steps. Several machine learning algorithms are implemented to classify whether a customer will churn (leave the service) or not.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Data Visualization](#data-visualization)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Customer churn prediction is crucial for businesses to retain customers by identifying those at risk of leaving. This project uses machine learning techniques to predict customer churn based on various features.

## Features

- Data preprocessing: Cleaning and preparing the customer churn data for modeling.
- Data visualization: Visualizing the distribution of features and their relationship with churn.
- Model training: Implementing various algorithms including K-Nearest Neighbors, Support Vector Machine, Random Forest, and Decision Tree to train a churn prediction model.
- Model evaluation: Assessing the performance of each model using accuracy metrics.

## Dataset

The dataset used in this project is the [Customer Churn Data](https://www.kaggle.com/shubhendra-singh/churn-modelling) from Kaggle. It contains information about customers and whether they have churned.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/Aanchal2707/customer-churn-prediction.git
    cd customer-churn-prediction
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Ensure you have the dataset file (`Churn_Modelling.csv`) in the project directory. If not, download it from the provided link and place it there.

2. Run the script to execute data preprocessing, visualization, model training, and evaluation:
    ```bash
    python churn_prediction.py
    ```

## Data Visualization

The project includes various data visualization steps to understand the distribution of features and their relationship with churn. Key visualizations include:

- Count plots showing the distribution of the target variable (`Exited`).
- Pie charts showing the distribution of gender.
- Bar plots showing the relationship between geography, gender, and churn.
- Histograms showing the distribution of age and other features.

## Model Training and Evaluation

The script `churn_prediction.py` performs the following steps:

1. Loads and preprocesses the data.
2. Visualizes the data to understand feature distributions and relationships.
3. Extracts features and splits the data into training and testing sets.
4. Trains several machine learning models including K-Nearest Neighbors (KNN), Support Vector Machine (SVM), Random Forest, and Decision Tree.
5. Evaluates each model using accuracy metrics.

## Results

The results of the model evaluations are summarized in a DataFrame showing the accuracy of each model:

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest
- Decision Tree

```python
models = pd.DataFrame({
    'name_model': ["KNN", "SVM", "Random Forest", "Decision Trees"],
    'accuracy_percentage': [percent1, percent2, percent3, percent4]
})
print(models)
```

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or suggestions! Happy coding!

---

**Note:** Replace `Aanchal2707` with your actual GitHub username in the clone URL.
