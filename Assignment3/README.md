# Assignment 1: Iris Flower Classification and Visualization  

## 📌 Objective  
The objective of this assignment is to classify **Iris flower species** using their sepal and petal measurements.  
We perform:  
- **Exploratory Data Analysis (EDA)** → To understand feature patterns with visualizations.  
- **Model Training** → Logistic Regression, Decision Tree, Random Forest, SVM.  
- **Model Evaluation** → Accuracy, Confusion Matrix, Classification Report.  
- **Visualization** → Pairplot, Boxplot, Heatmap, and Decision Boundaries.  

---

## 📊 Dataset  
- **Iris Dataset (in-built sklearn dataset)**  
  - **Features (Inputs):**  
    - Sepal Length (cm)  
    - Sepal Width (cm)  
    - Petal Length (cm)  
    - Petal Width (cm)  
  - **Target (Output):**  
    - Species → Setosa, Versicolor, Virginica  
- Total Samples: **150** (50 per species).  

---

## 🔎 Steps I Followed  

1. **Data Exploration**  
   - Loaded the Iris dataset and converted it into a DataFrame.  
   - Checked summary statistics with `df.describe()` to understand data spread.  
   - Visualized:  
     - **Pairplot** → Relationships between all feature pairs, color-coded by species.  
     - **Boxplot** → Distribution + median + outliers per species.  
     - **Heatmap (Correlation Matrix)** → Feature correlations.  

2. **Model Training**  
   - Split data into **80% training, 20% testing**.  
   - Trained models:  
     - Logistic Regression  
     - Decision Tree  
     - Random Forest  
     - SVM  

3. **Model Evaluation**  
   - Predictions made on test set.  
   - Evaluated using:  
     - **Accuracy Score**  
     - **Confusion Matrix (heatmap)**  
     - **Classification Report (precision, recall, F1-score)**  

4. **Visualization of Decision Boundaries**  
   - Plotted decision regions to show how models separate different flower species.  

---

## 📈 Results  

- **Logistic Regression Accuracy:** 100%  
- **Decision Tree Accuracy:** ~100%  
- **Random Forest Accuracy:** ~100%  
- **SVM Accuracy:** ~100%  

- **Confusion Matrix:**  
  - All test samples were correctly classified.  
  - No misclassifications observed.  

- **Classification Report:**  
  - Precision = 1.00  
  - Recall = 1.00  
  - F1-score = 1.00  

---

## 📝 Learning  

- Understood how to use **pairplot, boxplot, heatmap** for dataset understanding.  
- Learned the importance of **train-test split** in evaluating models on unseen data.  
- Explored **precision, recall, F1-score, accuracy** as evaluation metrics.  
- Understood **confusion matrix** as a scoreboard for classification.  
- Saw how decision boundaries visualize model performance.  

---

## ⚡ Conclusion  

- The Iris dataset is **small, clean, and well-separated**, making it ideal for learning classification.  
- All models achieved **100% accuracy** on this dataset.  
- **Petal length and width** were the strongest features for separating species.  
- Visualization made results intuitive and confirmed statistical findings.  
- This assignment showed how **EDA + ML models + visualization** together give a complete picture of classification.  
