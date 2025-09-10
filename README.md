# 🎯 Supervised Learning Project Collection

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-green.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-red.svg)](https://pandas.pydata.org/)

A comprehensive collection of **Supervised Learning** implementations covering various machine learning algorithms, data preprocessing techniques, and real-world applications. This repository serves as a complete learning resource for understanding and implementing supervised learning concepts from scratch.

## 📋 Table of Contents

- [🎯 Overview](#-overview)
- [🚀 Features](#-features)
- [🧠 Machine Learning Algorithms](#-machine-learning-algorithms)
- [📊 Datasets](#-datasets)
- [🛠️ Installation](#️-installation)
- [📖 Usage](#-usage)
- [📁 Project Structure](#-project-structure)
- [🔧 Model Serialization](#-model-serialization)
- [🎓 Learning Path](#-learning-path)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

## 🎯 Overview

This repository contains a comprehensive collection of **supervised learning** implementations using Python, scikit-learn, pandas, and other essential data science libraries. Each notebook demonstrates practical applications of machine learning algorithms on real-world datasets, making it perfect for:

- **Students** learning machine learning fundamentals
- **Data Scientists** looking for implementation references
- **Researchers** exploring different algorithmic approaches
- **Practitioners** seeking real-world examples

## 🚀 Features

✨ **Complete Algorithm Coverage**: Implementation of all major supervised learning algorithms  
📊 **Real-World Datasets**: Practical examples using diverse datasets  
🔄 **Data Preprocessing**: Comprehensive data cleaning and feature engineering  
📈 **Visualization**: Beautiful plots and charts for data insights  
💾 **Model Persistence**: Save and load trained models using joblib and pickle  
📝 **Detailed Documentation**: Well-commented code with explanations  
🎯 **Performance Metrics**: Evaluation using various metrics and validation techniques  

## 🧠 Machine Learning Algorithms

### 📈 Regression Algorithms
- **Linear Regression** - `LinearRegression.ipynb`, `LinearPractice.ipynb`
  - Simple and multiple linear regression
  - House price prediction using linear models
  - Feature scaling and normalization
  
- **Gradient Descent** - `Gradeint_decent.ipynb`, `Gradient_decent_exc.ipynb`
  - Implementation from scratch
  - Visualization of cost function optimization
  - Different learning rates comparison

### 🎯 Classification Algorithms
- **Logistic Regression** - `LogisticalRegression.ipynb`, `LogisticRegressionExc.ipynb`, `LogisticRegressionDigits.ipynb`
  - Binary and multiclass classification
  - Handwritten digits recognition
  - Decision boundary visualization
  
- **Decision Trees** - `DecisionTreeClassifier.ipynb`, `TitanicDecisionTree.ipynb`
  - Tree visualization and interpretation
  - Titanic survival prediction
  - Feature importance analysis
  
- **Random Forest** - `RandomForestClassifier.ipynb`, `randomForestIris.ipynb`
  - Ensemble method implementation
  - Iris species classification
  - Feature importance and model interpretation
  
- **Support Vector Machines (SVM)** - `SVMClassifier.ipynb`, `SVMDigits.ipynb`
  - Linear and non-linear SVM
  - Kernel trick implementation
  - Handwritten digits classification
  
- **Naive Bayes** - `Naive-Gaussian.ipynb`, `Naive-Wine.ipynb`
  - Gaussian Naive Bayes
  - Wine quality prediction
  - Probabilistic classification

### 🔍 Clustering Algorithms
- **K-Means Clustering** - `K-means.ipynb`, `K-means-Iris.ipynb`
  - Unsupervised learning implementation
  - Customer segmentation
  - Iris dataset clustering analysis

### 🛠️ Data Preprocessing
- **One-Hot Encoding** - `OneHotEncod.ipynb`, `Hotencode.ipynb`
  - Categorical variable handling
  - Feature encoding techniques
  - Data transformation pipelines

### 🎯 Special Applications
- **Spam Classification** - `Spam-classifier.ipynb`
  - Email spam detection
  - Text preprocessing and feature extraction
  - Natural Language Processing techniques

## 📊 Datasets

This project includes various real-world datasets for comprehensive learning:

### 🏠 **Real Estate & Housing**
- `homeprices.csv`, `homeprices _1.csv` - House price prediction
- `carprices.csv` - Automobile price analysis

### 👥 **Human Resources & Employment**
- `hiring.csv` - Hiring decision prediction
- `salaries.csv` - Salary prediction models
- `income.csv` - Income classification

### 🎓 **Education & Performance**
- `Student_Performance.csv` - Student academic performance analysis
- `test_scores.csv` - Test score prediction

### 🍽️ **Food & Restaurant Industry**
- `Swiggy.csv` - Food delivery platform data (1.2MB dataset)
- `Zomato.xlsx` - Restaurant analytics (2.3MB dataset)
- `menu.csv`, `Cleaned_menu.csv` - Menu data analysis

### 🚢 **Transportation**
- `titanic.csv` - Famous Titanic survival prediction dataset

### 📧 **Communication**
- `spam.csv` - Email spam detection dataset (480KB)

### 🏥 **Healthcare**
- `insurance_data.csv` - Medical insurance prediction

### 🏙️ **Geographic Data**
- `Indore_cleaned.csv` - City-specific dataset analysis (93KB)

## 🛠️ Installation

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab

### Quick Setup

1. **Clone the repository**
```bash
git clone https://github.com/MadhavGupta1506/Supervised-learning.git
cd Supervised-learning
```

2. **Install required packages**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

3. **Additional packages (used in specific notebooks)**
```bash
pip install word2number  # For text preprocessing
pip install openpyxl     # For Excel file reading
```

### Alternative: Using Conda
```bash
conda create -n ml-env python=3.8
conda activate ml-env
conda install pandas numpy scikit-learn matplotlib seaborn jupyter
```

## 📖 Usage

### 🚀 Getting Started

1. **Start Jupyter Notebook**
```bash
jupyter notebook
```

2. **Open any notebook** from the project directory

3. **Run the cells** sequentially to see the implementation

### 📚 Recommended Learning Path

#### **Beginners (Start Here)**
1. `LinearRegression.ipynb` - Learn regression basics
2. `LogisticalRegression.ipynb` - Understand classification
3. `DecisionTreeClassifier.ipynb` - Tree-based methods

#### **Intermediate**
4. `RandomForestClassifier.ipynb` - Ensemble methods
5. `SVMClassifier.ipynb` - Advanced classification
6. `Naive-Gaussian.ipynb` - Probabilistic models

#### **Advanced**
7. `Gradeint_decent.ipynb` - Optimization algorithms
8. `OneHotEncod.ipynb` - Feature engineering
9. `Spam-classifier.ipynb` - Real-world application

### 🎯 Example Usage

```python
# Load a dataset
import pandas as pd
df = pd.read_csv('homeprices.csv')

# Train a model
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X_train, y_train)

# Make predictions
predictions = model.predict(X_test)
```

## 📁 Project Structure

```
Supervised-learning/
│
├── 📊 Regression Models
│   ├── LinearRegression.ipynb          # Basic linear regression
│   ├── LinearPractice.ipynb           # Linear regression practice
│   ├── HousePrediction.ipynb          # House price prediction
│   ├── Gradeint_decent.ipynb          # Gradient descent optimization
│   └── Gradient_decent_exc.ipynb      # Advanced gradient descent
│
├── 🎯 Classification Models
│   ├── LogisticalRegression.ipynb      # Logistic regression basics
│   ├── LogisticRegressionExc.ipynb    # Advanced logistic regression
│   ├── LogisticRegressionDigits.ipynb # Digit classification
│   ├── DecisionTreeClassifier.ipynb   # Decision tree implementation
│   ├── TitanicDecisionTree.ipynb      # Titanic survival prediction
│   ├── RandomForestClassifier.ipynb   # Random forest ensemble
│   ├── randomForestIris.ipynb         # Iris classification with RF
│   ├── SVMClassifier.ipynb            # Support Vector Machine
│   ├── SVMDigits.ipynb               # SVM for digit recognition
│   ├── Naive-Gaussian.ipynb          # Gaussian Naive Bayes
│   └── Naive-Wine.ipynb              # Wine classification
│
├── 🔍 Clustering & Unsupervised
│   ├── K-means.ipynb                  # K-means clustering
│   └── K-means-Iris.ipynb            # Iris dataset clustering
│
├── 🛠️ Data Preprocessing
│   ├── OneHotEncod.ipynb             # One-hot encoding techniques
│   └── Hotencode.ipynb               # Hot encoding examples
│
├── 🎯 Applications
│   ├── Spam-classifier.ipynb          # Email spam detection
│   └── Untitled.ipynb               # Experimental notebook
│
├── 📊 Datasets
│   ├── homeprices.csv                # House pricing data
│   ├── carprices.csv                 # Car pricing data
│   ├── titanic.csv                   # Titanic passenger data
│   ├── spam.csv                      # Email spam dataset
│   ├── Student_Performance.csv       # Student academic data
│   ├── Swiggy.csv                    # Food delivery data
│   ├── Zomato.xlsx                   # Restaurant data
│   └── [other datasets...]
│
├── 💾 Saved Models
│   ├── model_joblib                  # Serialized model (joblib)
│   └── model_pickle                  # Serialized model (pickle)
│
└── 📁 Generated Files
    └── .ipynb_checkpoints/           # Jupyter checkpoint files
```

## 🔧 Model Serialization

The project demonstrates model persistence using two popular methods:

### Using Joblib (Recommended)
```python
import joblib

# Save model
joblib.dump(model, 'model_joblib')

# Load model
loaded_model = joblib.load('model_joblib')
```

### Using Pickle
```python
import pickle

# Save model
with open('model_pickle', 'wb') as f:
    pickle.dump(model, f)

# Load model
with open('model_pickle', 'rb') as f:
    loaded_model = pickle.load(f)
```

## 🎓 Learning Path

### 🌟 **Phase 1: Foundation (Weeks 1-2)**
- Linear Regression concepts and implementation
- Basic data preprocessing and visualization
- Understanding supervised vs unsupervised learning

### 🌟 **Phase 2: Classification (Weeks 3-4)**
- Logistic Regression for binary classification
- Decision Trees and interpretability
- Model evaluation metrics

### 🌟 **Phase 3: Advanced Algorithms (Weeks 5-6)**
- Ensemble methods (Random Forest)
- Support Vector Machines
- Naive Bayes for probabilistic classification

### 🌟 **Phase 4: Optimization & Engineering (Weeks 7-8)**
- Gradient Descent optimization
- Feature engineering and selection
- Model serialization and deployment

### 🌟 **Phase 5: Real-World Applications (Weeks 9-10)**
- Complete project: Spam classification
- Data preprocessing pipelines
- Performance optimization

## 🤝 Contributing

We welcome contributions to improve this learning resource! Here's how you can help:

### 🎯 **Ways to Contribute**
- 📚 Add new algorithm implementations
- 🐛 Fix bugs or improve existing code
- 📊 Add new datasets and examples
- 📝 Improve documentation and comments
- 🎨 Create visualizations and plots

### 📋 **Contribution Guidelines**
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-algorithm`)
3. Commit your changes (`git commit -am 'Add new algorithm'`)
4. Push to the branch (`git push origin feature/new-algorithm`)
5. Create a Pull Request

### 📝 **Code Style**
- Use clear, descriptive variable names
- Add comments explaining complex algorithms
- Include docstrings for functions
- Follow PEP 8 style guidelines

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🎉 Acknowledgments

- **Scikit-learn** community for excellent documentation
- **Pandas** team for powerful data manipulation tools  
- **Jupyter** project for interactive computing environment
- **Matplotlib/Seaborn** for beautiful visualizations

## 📞 Contact

**Madhav Gupta** - Project Maintainer
- GitHub: [@MadhavGupta1506](https://github.com/MadhavGupta1506)

---

⭐ **Star this repository** if you find it helpful for your machine learning journey!

🚀 **Happy Learning and Coding!** 🎯

---

*Last Updated: September 2024*