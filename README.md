# 🏘️ Nashville Housing Investment Analysis - Predictive Analytics
## 📊 Academic Project - ALY 6020: Predictive Analytics
**Institution:** Northeastern University  
**Course:** ALY 6020 - Predictive Analytics  
**Professor:** Yongqiang (Yong) Zhang  
**Term:** Fall 2024

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
