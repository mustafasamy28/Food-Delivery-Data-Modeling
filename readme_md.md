# Food Delivery Data Analysis Project

![Food Delivery Analytics](https://img.shields.io/badge/Analytics-Food%20Delivery-orange)
![Python](https://img.shields.io/badge/Python-3.7+-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.0+-yellow)
![Data Science](https://img.shields.io/badge/Data%20Science-Analysis-green)
![Machine Learning](https://img.shields.io/badge/ML-Classification-red)

## 📋 Project Overview

This project analyzes a comprehensive food delivery dataset to extract actionable insights for optimizing restaurant operations and planning strategic expansion. Using statistical analysis, data visualization, and machine learning techniques, the project identifies optimal restaurant locations, predicts order delays, and recommends the most profitable cuisine types.

## 🛠️ Skills & Technologies Used

- **Python** for data manipulation and analysis
- **Pandas** for data preprocessing and transformation
- **NumPy** for numerical operations
- **Matplotlib/Seaborn** for data visualization
- **Scikit-learn** for machine learning models
- **Statistical Analysis** for identifying patterns and correlations
- **Data Cleaning** for handling outliers and missing values
- **Feature Engineering** for model enhancement

## 📊 Data Description

The analysis is based on a food delivery dataset containing the following key information:
- Order details (date, time, status)
- Location information (customer district, branch district, distance)
- Time metrics (delivery time, estimation, delay)
- Cuisine types
- Performance indicators

## 🔍 Key Analyses & Findings

### 1. Location Analysis
- Identified Al Malga and Al Yasmin as top districts for new restaurant locations
- Al Yasmin leads in customer order volume (3,400+ orders)
- Al Malga leads in branch order volume (4,000+ orders)

### 2. Delay Prediction
- Built a high-accuracy classification model (100% accuracy on test data)
- Identified key delay indicators:
  - Geographic: Orders from Gbraya district have highest delay rate (0.82%)
  - Cuisine-specific: Healthy food orders experience highest delays
  - Temporal: Saturday orders have highest delay rates
  - Negative correlation between distance and delay

### 3. Cuisine Performance Analysis
- Fast food has highest order volume (10,000+ orders)
- Traditional food, sandwich, and pizza also highly popular (9,000+ orders each)
- Identified cuisine types with lowest delay rates

### 4. Time Analysis
- Evening hours show massive demand peak (55,000+ orders)
- Weekend days (Friday-Sunday) show significantly higher demand than weekdays

## 📈 Visualizations

The project includes several key visualizations:

### Top Customer Districts
![Top Customer Districts](images/top_customer_districts.png)
<!-- Original link: https://drive.google.com/file/d/16RsnUyN1LS78cGxEeRXkRn9jz1puIADM/view?usp=drive_link -->

### Branch District Distribution (Top 20)
![Branch District Distribution](images/branch_district_distribution.png)
<!-- Original link: https://drive.google.com/file/d/1VPCQ_fAv2fRpgAEzPgnvwiEma1nntu4P/view?usp=drive_link -->

### Relationship Between Distance and Delay
![Distance vs Delay](images/distance_vs_delay.png)
<!-- Original link: https://drive.google.com/file/d/1R1kPkpygd_0-Om0em-C3lJzAxzrdXwnA/view?usp=drive_link -->

### Time Analysis
![Time Analysis](images/time_analysis.png)
<!-- Original link: https://drive.google.com/file/d/19D-smNGkBBy2x6CTdV_W2XbBvtjhjQT9/view?usp=sharing -->

### Distribution of Orders by Time
![Orders by Time](images/orders_by_time.png)
<!-- Original link: https://drive.google.com/file/d/1Gszm5dGo8ujZD9JBX1MzbzRKey48soLv/view?usp=drive_link -->

### Cuisine Analysis
![Cuisine Analysis](images/cuisine_analysis.png)
<!-- Original link: https://drive.google.com/file/d/1ADPcPiunwAYyV7OkH7n8dfVh1O4fV6Kq/view?usp=drive_link -->

### Cuisine Performance Across Branch Districts
![Cuisine Performance Heatmap](images/cuisine_performance_heatmap.png)
<!-- Original link: https://drive.google.com/file/d/1CSrJN9JJ7HExSWruqIWH4Jf74NEuFVFs/view?usp=drive_link -->

### Delay Analysis (Top 10 Branch Districts)
![Delay Analysis by District](images/delay_analysis_districts.png)
<!-- Original link: https://drive.google.com/file/d/1n5UD5ohdZuj42HJgT-QEC-PBtlmFYryh/view?usp=drive_link -->

### Delay by Cuisine
![Delay by Cuisine](images/delay_by_cuisine.png)
<!-- Original link: https://drive.google.com/file/d/1yB2qQsTQuMEGk1FnPpfDOeBpDY8wj9Rl/view?usp=drive_link -->

### Delay by Day
![Delay by Day](images/delay_by_day.png)
<!-- Original link: https://drive.google.com/file/d/1MBW-lpwuww_BnaelGs2V6J7jLA8OsiCE/view?usp=drive_link -->

### Correlation Matrix
![Correlation Matrix](images/correlation_matrix.png)
<!-- Original link: https://drive.google.com/file/d/1yhcwzk-4vzL7KjjfoifAbMF2IiXLz2bs/view?usp=drive_link -->

### Best Location Analysis
![Best Location Analysis](images/best_location_analysis.png)
<!-- Original link: https://drive.google.com/file/d/16liGiV1e7OECFESD7liisG-2vQOPdsDw/view?usp=drive_link -->

## 💡 Strategic Recommendations

1. **Best Location for New Restaurant:** Open in Al Malga or Al Yasmin districts
2. **Recommended Restaurant Type:** Fast food restaurant with traditional food options and sandwiches
3. **Operational Strategy:** Focus on dinner service and ensure full staffing on weekends

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Required libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/food-delivery-analysis.git

# Navigate to project directory
cd food-delivery-analysis

# Install required packages
pip install -r requirements.txt

# Run the analysis
python main.py
```

### Project Structure

```
food-delivery-analysis/
├── data/                # Data directory (not included in repo)
│   └── README.md        # Information about how to obtain the data
├── notebooks/           # Jupyter notebooks for analysis
│   ├── data_cleaning.ipynb
│   ├── exploratory_analysis.ipynb
│   └── model_building.ipynb
├── src/                 # Source code
│   ├── preprocessing.py # Data preprocessing functions
│   ├── visualization.py # Visualization functions
│   └── modeling.py      # Machine learning models
├── results/             # Output visualizations and results
├── README.md            # Project documentation
├── requirements.txt     # Required packages
└── main.py              # Main execution script
```

## 📋 Sample Output

```
----- Best Location Analysis -----

Top 10 Districts for Restaurant Location:
      district  customer_orders  branch_orders  success_ratio  composite_score
0     Al Malga            2743.0        4029.0       1.468832         0.951825
1    Al Yasmin            3402.0        2734.0       0.803645         0.883511
2  Al Nakheel             2180.0        2562.0       1.175229         0.723850
3     Al Rabwh            1947.0        2343.0       1.203390         0.671252
4   Al Mansora            1843.0        1987.0       1.078133         0.589977
5     Al Aridh            1601.0        1781.0       1.112430         0.531158
6      Nakheel            1425.0        1677.0       1.176842         0.498131
7     Al Nahdh            1389.0        1520.0       1.094313         0.463161
8     Al Mrooj            1233.0        1456.0       1.180858         0.441764
9    Al Solayy            1193.0        1377.0       1.154233         0.421612
```

## 🧠 Machine Learning Model Performance

```
----- Order Delay Prediction Model -----
Training the model... ✅
Model Accuracy: 1.0000

📋 Classification Report:
              precision    recall  f1-score   support
           0       1.00      1.00      1.00      9692
           1       1.00      1.00      1.00      7771
    accuracy                           1.00     17463
   macro avg       1.00      1.00      1.00     17463
weighted avg       1.00      1.00      1.00     17463
```

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

