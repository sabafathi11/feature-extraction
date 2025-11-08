# 🧠 Feature Extraction and Dimensionality Reduction Analysis

This project presents a comparative study of various **feature extraction and dimensionality reduction algorithms** — including **PCA**, **ICA**, **SVD**, **RFE**, and **SelectKBest** — on three classical machine learning tasks: **classification**, **regression**, and **clustering**.  
The goal is to analyze how feature extraction impacts model **accuracy**, **speed**, and **stability** across different datasets.

---

## 📊 Datasets
Three well-known public datasets were used, all available from `scikit-learn`:
- 🧬 **Breast Cancer Wisconsin Dataset** – Classification task  
- 🏠 **Boston Housing Dataset** – Regression task  
- 🌸 **Iris Dataset** – Clustering task  

Each dataset was explored using `pandas` to examine feature structure and statistical properties.

---

## ⚙️ Methodology
1. **Data Preprocessing**  
   - Features were standardized using `StandardScaler` for better numerical stability.  
2. **Collinearity Analysis**  
   - Correlation heatmaps were generated to visualize feature dependencies and detect redundancy.  
3. **Feature Extraction**  
   - Five algorithms were applied: `PCA`, `ICA`, `SVD`, `RFE`, and `SelectKBest`.  
   - The number of components was determined based on **explained variance ratio (95%)** for PCA and aligned for other methods.  
4. **Model Evaluation**  
   - Each transformed dataset was evaluated with multiple models such as `KNN`, `RandomForest`, and `LinearRegression`.  
   - Accuracy, prediction time, and model stability were compared against the original data.

---

## 📈 Results
- Dimensionality reduction generally **improved computational efficiency** with minimal or no loss in accuracy.  
- The **PCA** algorithm provided the best trade-off between performance and interpretability.  
- The **Random Forest** model showed **robustness against feature collinearity**, maintaining high accuracy even on non-reduced datasets.  
- Visual comparisons (accuracy vs. time) are included in the report for each model.

