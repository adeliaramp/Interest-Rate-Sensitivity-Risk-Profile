# Interest Rate Sensitivity Based on Users' Risk Profile

This project is an analysis of simulated default probabilities by risk profile for a fixed-rate credit product. The objective is to explore repayment behavior and provide actionable insights for optimizing loan portfolios. The analysis incorporates exploratory data visualization, undersampling techniques to address class imbalance, and logistic regression modeling.

## **Table of Contents**
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Analysis and Visualizations](#analysis-and-visualizations)
- [Model Evaluation](#model-evaluation)
- [Insights and Recommendations](#insights-and-recommendations)

---

## **Project Overview**
In this project, we analyze simulated default probabilities for borrowers categorized into three risk profiles: **Low**, **Medium**, and **High**. The analysis includes:
1. Exploratory Data Analysis (EDA) to identify patterns.
2. Logistic regression modeling after undersampling the dataset to balance class distribution.
3. Evaluation of model performance using classification metrics and AUC-ROC score.
4. Visualization of default probabilities by risk profile to derive actionable business insights.

---

## **Dataset Description**
The dataset used in this project includes the following key features:
- **RiskProfile**: Categorized into Low, Medium, and High.
- **DefaultProbability**: Simulated probability of default.
- **LoanAmount**: Borrower’s loan size.
- **Income**: Borrower’s monthly income.

The dataset includes 1,000 simulated rows to mimic realistic credit data.

---

## **Analysis and Visualizations**
### **Key Visualizations**:
1. **Boxplot of Default Probabilities by Risk Profile**:
   - Highlights the spread, median, and variability in default probabilities for each risk group.

### **Highlights**:
- **Low-Risk Borrowers**: Stable repayment behavior with low default probabilities.
- **Medium-Risk Borrowers**: Moderate default probabilities with higher variability.
- **High-Risk Borrowers**: Significant risk with the highest median and variability.

---

## **Model Evaluation**
The logistic regression model was evaluated using the following metrics after applying undersampling:

| Metric         | Class 0 (Non-Default) | Class 1 (Default) |
|----------------|-----------------------|-------------------|
| **Precision**  | 0.91                 | 0.27              |
| **Recall**     | 0.71                 | 0.61              |
| **F1-Score**   | 0.80                 | 0.37              |
| **Accuracy**   | 70%                  | -                 |
| **AUC-ROC**    | -                    | 0.6884            |

### **Observations**:
- Good performance on identifying non-defaults (Class 0).
- Moderate recall for identifying defaults (Class 1).
- AUC-ROC score of 0.6884 suggests room for improvement in differentiating between classes.

---

## **Insights and Recommendations**
### **Insights**:
1. **Low-Risk Borrowers**:
   - Low default probabilities indicate stable repayment behavior.
2. **Medium-Risk Borrowers**:
   - Higher variability in default probabilities requires closer monitoring.
3. **High-Risk Borrowers**:
   - The highest default probabilities and variability suggest significant risk.

### **Recommendations**:
1. **Low-Risk Borrowers**:
   - Expand loan offerings and provide loyalty incentives.
2. **Medium-Risk Borrowers**:
   - Offer flexible repayment plans and monitor repayment patterns closely.
3. **High-Risk Borrowers**:
   - Restrict loan approvals and offer financial literacy programs to mitigate risk.

Thank you for exploring this project! Feedback and contributions are welcome.

