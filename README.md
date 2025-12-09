# 🏘️ Nashville Housing Investment Analysis - Predictive Analytics
---
## 🎯 Executive Summary

This project analyzes Nashville's booming real estate market (2013-2016) to identify investment opportunities through machine learning. During this period, Nashville experienced a **30% three-year appreciation rate**, making it crucial to identify undervalued properties for strategic investment.

### 🔍 Business Problem
A real estate investment firm needs to identify properties that are underpriced relative to their true market value to maximize ROI in Nashville's competitive market.

### 💡 Solution Approach
Developed and compared **5 machine learning models** to predict whether properties sold above or below their assessed value, achieving up to **75.47% accuracy** with Gradient Boosting.

## 📈 Key Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|---------|----------|
| **Gradient Boosting** 🏆 | **75.47%** | 0.76 | 0.98 | 0.86 |
| Neural Network | 75.27% | 0.76 | 0.98 | 0.86 |
| Logistic Regression | 75.05% | 0.75 | 0.99 | 0.86 |
| Ensemble (Voting) | 75.13% | 0.76 | 0.98 | 0.86 |
| Random Forest | 71.35% | 0.76 | 0.90 | 0.83 |
| Decision Tree | 63.28% | 0.77 | 0.73 | 0.75 |

## 🔬 Methodology

### Data Pipeline
```python
Raw Data (56,000+ properties) → Cleaning → Feature Engineering → 
→ Model Training → Evaluation → Investment Recommendations
```

### Data Processing Highlights
- **Initial Dataset:** 56,477 properties with 31 features
- **Final Dataset:** 25,132 properties with 25,553 features (after encoding)
- **Target Variable:** Binary classification (Over_Under valued)
- **Key Techniques:**
  - Z-score outlier removal (threshold=3)
  - Median/mode imputation for missing values
  - One-hot encoding for categorical variables
  - StandardScaler normalization

## 📊 Visualizations

### Distribution Analysis
![Distribution](reports/figures/distribution_plot.png)

### Feature Correlations
![Correlation](reports/figures/correlation_heatmap.png)

### Model Performance Comparison
![Model Comparison](reports/figures/model_comparison.png)

## 🛠️ Technical Implementation

### Technologies Used
- **Programming:** Python 3.8+
- **Data Processing:** Pandas, NumPy, SciPy
- **Machine Learning:** Scikit-learn
- **Visualization:** Matplotlib, Seaborn
- **Statistical Analysis:** Z-score outlier detection, correlation analysis

### Models Implemented
1. **Logistic Regression** - Baseline model with interpretability
2. **Decision Tree** - Non-linear patterns with visualization
3. **Random Forest** - Ensemble of 100 trees
4. **Gradient Boosting** - Best performer with iterative optimization
5. **Neural Network** - MLPClassifier with 50 hidden units
6. **Ensemble Voting** - Combining all models (Bonus)

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.8+
Jupyter Notebook
Git LFS (for large files)
```

### Installation & Usage

1. **Clone the repository**
```bash
git clone https://github.com/arpitaoberoi/nashville-housing-analysis.git
cd nashville-housing-analysis
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Download the dataset**
```bash
# Download from Kaggle
kaggle datasets download -d tmthyjames/nashville-housing-data
unzip nashville-housing-data.zip -d data/raw/
```

4. **Run the analysis**
```bash
jupyter notebook notebooks/Nashville_Project.ipynb
```

# 📊 Key Findings & Investment Recommendations

### 🎯 Strategic Insights
1. **Gradient Boosting model identified key value indicators:**
   - Land Value (strongest predictor)
   - Building Value
   - Finished Area
   - Number of Bedrooms/Bathrooms

2. **Investment Strategy:**
   - Target properties with high land-to-building value ratios
   - Focus on properties with 3-4 bedrooms (optimal for market demand)
   - Prioritize finished areas between 1,500-2,500 sq ft

3. **Market Patterns:**
   - 75% of properties sold above assessed value (seller's market)
   - Properties in certain tax districts show consistent undervaluation


## 🏆 Academic Achievement

This project was completed as part of the **MS in Data Analytics** program at Northeastern University, demonstrating proficiency in:
- Advanced predictive modeling techniques
- Business-oriented data analysis
- Statistical validation and testing
- Professional report writing
- Real-world problem solving

## 📈 Future Enhancements

- [ ] Implement XGBoost for potentially better performance
- [ ] Add geographic clustering analysis
- [ ] Create interactive dashboard with Plotly
- [ ] Implement time-series forecasting for price trends
- [ ] Add feature importance analysis with SHAP values

## 🤝 Contributing

While this is an academic project, suggestions and feedback are welcome! Please feel free to:
- Open an issue for bugs or suggestions
- Fork the repository for your own analysis
- Star ⭐ the repository if you found it helpful

## 📄 License

This project is licensed under the MIT License - see the [https://www.kaggle.com/datasets/tmthyjames/nashville-housing-data] file for details.

## 📬 Contact

**Arpita Oberoi**  
MS Data Analytics Candidate | Northeastern University  
- 📧 Email: arpitaoberoi5@gmail.com
- 💼 LinkedIn: [https://www.linkedin.com/in/arpita-oberoi/]
- 🌐 GitHub: [https://github.com/Arpita0511]

## 🙏 Acknowledgments

- Professor Yongqiang Zhang for guidance and feedback
- Northeastern University's ALY 6020 course framework
- Timothy James for the Nashville Housing dataset (Kaggle)
- Scikit-learn community for excellent documentation

---
⭐ **Note:** This project achieved excellent results in identifying undervalued properties with 75.47% accuracy, 
providing actionable insights for real estate investment decisions.
