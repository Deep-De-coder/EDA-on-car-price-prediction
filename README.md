# Car Price Prediction - Exploratory Data Analysis (EDA)

## 📋 Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on a car price prediction dataset. The analysis explores various factors that influence car prices, including vehicle specifications, market categories, and performance metrics.

## 🎯 Project Objectives

- Analyze the relationship between car features and MSRP (Manufacturer's Suggested Retail Price)
- Identify key factors that influence car pricing
- Perform data cleaning and preprocessing
- Create visualizations to understand data patterns and correlations
- Generate insights for car price prediction models

## 📊 Dataset Information

**Dataset:** `data.csv`
- **Size:** 11,914 records × 16 features
- **Target Variable:** MSRP (Manufacturer's Suggested Retail Price)
- **Features:** 15 independent variables

### Dataset Features

| Feature | Description | Type |
|---------|-------------|------|
| Make | Car manufacturer | Categorical |
| Model | Car model name | Categorical |
| Year | Manufacturing year | Numerical |
| Engine Fuel Type | Type of fuel required | Categorical |
| Engine HP | Horsepower rating | Numerical |
| Engine Cylinders | Number of cylinders | Numerical |
| Transmission Type | Transmission system | Categorical |
| Driven_Wheels | Wheel drive configuration | Categorical |
| Number of Doors | Number of doors | Numerical |
| Market Category | Market segment classification | Categorical |
| Vehicle Size | Size category | Categorical |
| Vehicle Style | Body style | Categorical |
| Highway MPG | Highway fuel efficiency | Numerical |
| City MPG | City fuel efficiency | Numerical |
| Popularity | Popularity score | Numerical |
| MSRP | Manufacturer's suggested retail price | Numerical (Target) |

## 📁 Project Structure

```
EDA-on-car-price-prediction/
├── README.md                                    # Project documentation
├── data.csv                                     # Raw dataset
├── Car_Price_Prediction_EDA.ipynb              # Main EDA notebook
├── Car_Price_Prediction_EDA_withcomments.ipynb # EDA notebook with detailed comments
└── BDA-MiniProject-Report.pdf                  # Project report (PDF)
```

## 🔧 Data Preprocessing Steps

1. **Data Loading & Initial Exploration**
   - Load dataset and examine basic statistics
   - Check data shape and column information

2. **Data Cleaning**
   - Standardize column names (lowercase, replace spaces with underscores)
   - Handle missing values:
     - Market Category: Fill with mode
     - Engine Fuel Type: Fill with mode
     - Engine HP: Fill with mean
     - Engine Cylinders: Fill with median
     - Number of Doors: Fill with median
   - Remove duplicate records

3. **Feature Engineering**
   - Categorize variables into numerical and categorical
   - Standardize categorical variable values

## 📈 Analysis Components

### 1. Data Quality Assessment
- Missing value analysis and treatment
- Duplicate record identification and removal
- Data type verification

### 2. Statistical Analysis
- Descriptive statistics for all variables
- Correlation analysis between numerical features
- Distribution analysis of target variable (MSRP)

### 3. Visualization Analysis
- **Distribution Plots:** For all numerical variables
- **Correlation Heatmap:** To identify feature relationships
- **Scatter Plots:** MSRP vs numerical features
- **Bar Plots:** Categorical variables vs MSRP

### 4. Key Insights
- Price distribution patterns
- Feature correlations with MSRP
- Categorical variable impact on pricing
- Market category analysis

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Basic plotting
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## 📊 Key Findings

### Data Characteristics
- **Dataset Size:** 11,914 cars with 16 features
- **Price Range:** Wide range from $2,000 to high-end luxury vehicles
- **Manufacturers:** 48 different car makes
- **Models:** 914 unique car models
- **Year Range:** 28 years of manufacturing data

### Missing Data
- Market Category: Some missing values (filled with mode)
- Engine Fuel Type: Minor missing values (filled with mode)
- Engine HP: Missing values (filled with mean)
- Engine Cylinders: Missing values (filled with median)
- Number of Doors: Missing values (filled with median)

### Data Quality
- Duplicate records identified and removed
- All missing values successfully treated
- Data types properly categorized

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Analysis
1. Clone or download the project files
2. Ensure `data.csv` is in the project directory
3. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Run either:
   - `Car_Price_Prediction_EDA.ipynb` (Main analysis)
   - `Car_Price_Prediction_EDA_withcomments.ipynb` (Detailed version with comments)

## 📋 Usage

1. **For Basic Analysis:** Use `Car_Price_Prediction_EDA.ipynb`
2. **For Detailed Learning:** Use `Car_Price_Prediction_EDA_withcomments.ipynb`
3. **For Project Report:** Refer to `BDA-MiniProject-Report.pdf`

## 🎓 Educational Value

This project demonstrates:
- Comprehensive EDA workflow
- Data cleaning and preprocessing techniques
- Statistical analysis and visualization
- Feature engineering approaches
- Real-world data analysis skills

## 📝 Notes

- The analysis uses Google Colab environment (as indicated by the file upload code)
- All visualizations use a consistent color scheme (copper theme)
- The project includes both commented and non-commented versions for different learning needs

## 🤝 Contributing

Feel free to contribute by:
- Improving visualizations
- Adding additional analysis techniques
- Enhancing documentation
- Suggesting new features

## 📄 License

This project is for educational purposes and data analysis demonstration.

---

**Note:** This project is part of a Big Data Analytics mini-project focusing on exploratory data analysis techniques for car price prediction.