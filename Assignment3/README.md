# 🌸 Iris Flower Classification

## 📌 Objective
Classify iris flowers into **Setosa, Versicolor, Virginica** using petal and sepal measurements.  
This project demonstrates **EDA, visualization, and ML classification models**.

---

## 📂 Dataset
- **Source**: `sklearn.datasets.load_iris()`  
- **Features**:  
  - Sepal length  
  - Sepal width  
  - Petal length  
  - Petal width  
- **Target**: Species (Setosa, Versicolor, Virginica)  

---

## 🧪 Steps Performed

### 1. Exploratory Data Analysis (EDA)
- 📊 **Class distribution** → verified balanced dataset.  
- 🔎 **Pair plots** → clear separation of species by petal length/width.  
- 📦 **Box plots** → feature comparison across species.  
- 🔥 **Correlation heatmap** → petal length and width highly correlated.  

### 2. Model Training
- **Train-test split**: 80% training, 20% testing.  
- Algorithm used: **Logistic Regression**.  

### 3. Evaluation
- ✅ **Accuracy**: ~95–97% (depending on split).  
- 📉 **Confusion Matrix**: shows very few misclassifications.  
- 📑 **Classification Report**: high precision, recall, and f1-score across all classes.  

---

## 📊 Visualizations
- Class distribution plot  
- Pair plots (features colored by species)  
- Box plots (feature distribution by species)  
- Correlation heatmap  
- Confusion matrix heatmap  

---

## ⚙️ Tech Stack
- **Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  

---

## 🚀 Key Insights
- Petal features are the strongest predictors for classification.  
- Logistic Regression performs well on this dataset due to clear class separability.  
- This dataset is a great starting point for understanding **classification models**.  

---

