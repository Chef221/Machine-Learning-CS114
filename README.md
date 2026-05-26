# NBA Game Predictor

A comprehensive machine learning project for predicting NBA game outcomes using advanced feature engineering and ensemble models.

## 📊 Project Overview

This project develops predictive models for NBA games by analyzing historical game statistics, team performance metrics, and contextual features. The solution includes multiple model iterations (V1, V2, V3) with progressive improvements in feature engineering and model architecture.

### Key Components

- **Data EDA**: Exploratory data analysis and data preparation
- **Feature Engineering**: Multiple versions (V1, V2, V3) of feature engineering pipelines
- **Modeling**: Ensemble models using XGBoost and LightGBM
- **NBA Predictor App**: Interactive Streamlit web application for game predictions

## 🏗️ Project Structure

```
CS114_CK/
├── data_eda/                           # Data exploration and cleaning
│   ├── CrawlingData.ipynb             # Web scraping and data collection
│   ├── EDA.ipynb                      # Exploratory data analysis
│   └── nba_data/                      # Raw datasets
│
├── FeatureEngineering/                # Feature development iterations
│   ├── V1/                            # Version 1 features
│   │   ├── code.ipynb
│   │   └── output/
│   │       ├── nba_model_ready_v1.csv
│   │       ├── feature_config_v1.json
│   │       └── eval_*.csv
│   │
│   └── V2/                            # Version 2 features (improved)
│       ├── code.ipynb
│       └── output/
│           ├── nba_model_ready_v2.csv
│           ├── feature_config_v2.json
│           └── eval_*.csv
│
├── Modeling/                          # Model training and evaluation
│   ├── V1/
│   │   └── code.ipynb                # V1 model development
│   │
│   └── V2/
│       └── code.ipynb                # V2 model improvements
│
├── V3-HuongMoRong/                    # Latest iteration (V3)
│   ├── Featurev3.ipynb               # V3 feature engineering
│   └── modelv3.ipynb                 # V3 model training
│
├── NBA_app/                           # Streamlit web application
│   ├── app.py                         # Main application
│   ├── requirements.txt               # Python dependencies
│   ├── nba_model_ready_v3.csv        # Feature dataset
│   └── feature_config_v3.json        # Feature configuration
│
├── Chronos-HuongMoRong/               # Additional model experiments
│   ├── chronos2-v2.ipynb
│   └── v1-chronos.ipynb
│
└── README.md                          # This file
```

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or higher
- pip or conda package manager
- Git

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/CS114_CK.git
   cd CS114_CK
   ```

2. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r NBA_app/requirements.txt
   # For Jupyter notebooks
   pip install jupyter matplotlib seaborn
   ```

### Running the Application

```bash
cd NBA_app
streamlit run app.py
```

The app will open at `http://localhost:8501`

## 📚 Workflow

### 1. Data Collection & EDA (`data_eda/`)

- Web scraping of NBA statistics
- Data cleaning and validation
- Statistical analysis and visualization

### 2. Feature Engineering (`FeatureEngineering/`)

- **V1**: Initial feature set with basic aggregations
- **V2**: Enhanced features with advanced metrics
- **V3**: Optimized features for production models

### 3. Model Development (`Modeling/`)

- Ensemble models combining XGBoost and LightGBM
- Hyperparameter tuning
- Cross-validation and performance evaluation

### 4. Production Deployment (`NBA_app/`)

- Interactive Streamlit interface
- Real-time predictions
- Model performance visualization

## 🤖 Models & Technologies

### Machine Learning Libraries

- **scikit-learn**: Data preprocessing and evaluation metrics
- **XGBoost**: Gradient boosting model
- **LightGBM**: Fast gradient boosting model
- **joblib**: Model serialization

### Data Processing

- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations

### Frontend

- **Streamlit**: Interactive web application framework

## 📈 Model Versions

| Version | Features                     | Accuracy | Status      |
| ------- | ---------------------------- | -------- | ----------- |
| V1      | Basic stats aggregations     | ~70%     | Development |
| V2      | Advanced contextual features | ~75%     | Development |
| V3      | Optimized ensemble features  | ~78%     | Production  |

## 📊 Data Features

The project uses multiple feature types:

- **Basic Stats**: Points, rebounds, assists, turnovers
- **Team Metrics**: Win-loss records, point differentials
- **Contextual Features**: Home/away, rest days, injury reports
- **Advanced Analytics**: Player efficiency ratings, pace-adjusted metrics

## 🔍 How to Use the Notebooks

1. **EDA Exploration**: Start with `data_eda/EDA.ipynb`
2. **Feature Development**: Review `FeatureEngineering/V1-V3/code.ipynb`
3. **Model Training**: Check `Modeling/V1-V2/code.ipynb`
4. **Latest Model**: Review `V3-HuongMoRong/modelv3.ipynb`

## 📁 Key Output Files

- `nba_model_ready_v*.csv`: Processed datasets ready for modeling
- `feature_config_v*.json`: Feature definitions and configurations
- `eval_train_v*.csv` / `eval_test_v*.csv`: Model evaluation results

## 🎯 Next Steps

- [ ] Expand dataset with recent 2024-25 season games
- [ ] Implement real-time API integration for live predictions
- [ ] Add player injury tracking
- [ ] Develop ensemble voting mechanism
- [ ] Create REST API for external consumption
- [ ] Deploy to cloud platform

## 📝 License

This project is part of CS114 coursework.

## 👤 Author

HuongMoRong

## 📧 Contact

For questions or collaboration, please reach out through GitHub issues.

---

**Last Updated**: May 2026
