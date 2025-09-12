# Airbnb Price Prediction

A comprehensive machine learning project that predicts Airbnb rental prices using various regression models, including Linear Regression, Ridge Regression, ElasticNet, and XGBoost.

## 📋 Project Overview

This project aims to predict Airbnb listing prices based on features such as location, property type, amenities, and host characteristics. By leveraging multiple machine learning algorithms, we compare their performance to identify the most effective approach for price prediction in the short-term rental market.

## 🎯 Objectives

- Develop accurate price prediction models for Airbnb listings
- Compare the performance of different regression algorithms
- Provide insights into key factors affecting rental prices
- Create a reusable framework for price prediction analysis

## 📊 Dataset Description

The dataset contains information about Airbnb listings with the following key features:

### Target Variable

- **Price**: The rental price per night (continuous variable)

### Feature Categories

- **Property Features**: Property type, room type, accommodates, bedrooms, bathrooms, beds
- **Location Features**: Neighborhood, latitude, longitude, city-specific attributes
- **Host Features**: Host response time, host response rate, host acceptance rate, superhost status
- **Booking Features**: Minimum nights, maximum nights, availability
- **Review Features**: Number of reviews, review scores (overall, cleanliness, check-in, communication, location, value)
- **Amenities**: WiFi, kitchen, parking, pool, gym, etc.

### Data Preprocessing

- Handle missing values using appropriate imputation strategies
- Encode categorical variables (one-hot encoding, label encoding)
- Feature scaling and normalization
- Remove outliers and anomalous data points
- Feature selection and engineering

## 🤖 Models Implemented

### 1. Linear Regression
- **Description**: Models a basic linear relationship
- **Use Case**: Serves as a baseline for comparison
- **Advantages**: Simple, interpretable, fast training

### 2. Ridge Regression
- **Description**: Linear regression with L2 regularization
- **Use Case**: Handles multicollinearity and reduces overfitting
- **Advantages**: Handles correlated features, reduces overfitting

### 3. ElasticNet Regression
- **Description**: Combines L1 and L2 regularization
- **Use Case**: Feature selection with regularization
- **Advantages**: Automatic feature selection, good for grouped features

### 4. XGBoost
- **Description**: Gradient boosting decision trees
- **Use Case**: Captures complex non-linear relationships
- **Advantages**: High performance, handles missing values, reveals feature importance

## 📈 Model Performance

### Evaluation Metrics

- **Mean Absolute Error (MAE)**: Average absolute difference between predicted and actual prices
- **Mean Squared Error (MSE)**: Average squared difference between predicted and actual prices
- **Root Mean Squared Error (RMSE)**: Square root of MSE, in same units as target
- **R² Score**: Coefficient of determination, proportion of variance explained
- **Mean Absolute Percentage Error (MAPE)**: Average percentage error

### Performance Results

| Model               | MAE  | RMSE   | R² Score | MAPE |
|---------------------|------|--------|----------|------|
| Linear Regression   | TBD  | 0.4033 | 0.6703   | TBD  |
| Ridge Regression    | TBD  | 0.4033 | 0.6704   | TBD  |
| ElasticNet          | TBD  | 0.4074 | 0.6636   | TBD  |
| XGBoost             | TBD  | 0.3727 | 0.7185   | TBD  |

*Note: Performance metrics will be updated after model training and evaluation.*

### Key Findings

- Feature importance analysis reveals the top price-influencing factors
- Model comparison highlights trade-offs between interpretability and performance
- Cross-validation ensures robust performance estimates

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Amanyadav-07/Airbnb-Price-Prediction.git
   cd Airbnb-Price-Prediction
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. **Data Preparation**
   - Place your Airbnb dataset in the `data/` directory
   - Ensure the dataset follows the expected format

2. **Run the Analysis**
   - Execute the main analysis script:
     ```bash
     python main.py
     ```
   - Or run individual notebooks:
     ```bash
     jupyter notebook
     ```

3. **View Results**
   - Model performance metrics will be displayed in the console
   - Visualizations and plots will be saved in the `outputs/` directory
   - Model artifacts will be saved in the `models/` directory

## 📁 Project Structure

```
Airbnb-Price-Prediction/
├── data/                   # Dataset files
├── notebooks/              # Jupyter notebooks for analysis
├── src/                    # Source code modules
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── models.py
│   └── evaluation.py
├── outputs/                # Generated plots and results
├── models/                 # Saved model artifacts
├── requirements.txt        # Project dependencies
├── main.py                # Main execution script
├── README.md              # Project documentation
└── .gitignore             # Git ignore file
```

## 🛠️ Dependencies

- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib**: Basic plotting and visualization
- **seaborn**: Statistical data visualization
- **scikit-learn**: Machine learning algorithms and tools
- **xgboost**: Gradient boosting framework

## 📝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Aman Kumar Yadav**  
GitHub: [@Amanyadav-07](https://github.com/Amanyadav-07)

## 🙏 Acknowledgments

- Airbnb for providing publicly available data
- Open source community for excellent machine learning libraries
- Contributors and collaborators who help improve this project