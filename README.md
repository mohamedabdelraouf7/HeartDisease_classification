# Heart Disease Classification Using Machine Learning

This project is part of the coursework for **CSE381 - Introduction to Machine Learning** at Future University in Egypt. It applies multiple machine learning techniques to classify whether a person has heart disease, based on medical features. The models are trained and validated using hyperparameter tuning and evaluated with performance metrics like accuracy, precision, recall, and F1-score.

👥 Team 

Alaa Yasser Fathy Bekhit & Mohamed Ahmed Abdelraouf    


## 📁 Files

- `HeartDisease_classification.ipynb`: The main Jupyter Notebook containing preprocessing, model building, and evaluation.
- `Project_Documentation.pdf`: Full project report with analysis, visualizations, and observations.
- `README.md`: Project overview and instructions.

## 🧪 Dataset Description

The dataset consists of 918 samples with clinical attributes such as:

- Age, RestingBP, Cholesterol, FastingBS, MaxHR, Oldpeak, Sex, ChestPainType, RestingECG, ExerciseAngina, ST_Slope
- Target: `HeartDisease` (0 = No, 1 = Yes)

### Key Observations:

- Mean age: 53.5 years.
- Heart disease prevalence: ~55%.
- Correlation: `Oldpeak` (0.4), `MaxHR` (-0.4), `Age` (0.28) with the target.

## 🧼 Data Preprocessing

- No missing or duplicate values.
- Outliers detected and capped using IQR method.
- Features scaled using `StandardScaler`.
- Dimensionality reduced using PCA for visualization.

## 🧠 Models and Performance

All models were tuned using `GridSearchCV` and evaluated on validation and test sets.

| Model          | Accuracy | Precision | Recall | F1-Score |
|----------------|----------|-----------|--------|----------|
| **SVM**        | 0.88     | 0.89      | 0.88   | 0.88     |
| **Naive Bayes**| 0.88     | 0.90      | 0.87   | 0.88     |
| **KNN**        | 0.87     | 0.87      | 0.87   | 0.87     |
| **Decision Tree** | 0.85  | 0.85      | 0.85   | 0.85     |

## 🔍 Insights

- **Naive Bayes** had the highest accuracy and precision.
- **SVM** offered the best recall, and was competitive overall.
- **KNN** and **Decision Tree** also performed well, but with slightly lower scores.
- Visualizations like PCA plots, correlation matrices, confusion matrices, and dendrograms were used to interpret model behavior and data structure.

## 🔧 Tools and Libraries

- Python, Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`, `fast_ml`
- Machine Learning techniques: PCA, GridSearchCV, classification metrics

## 🧰 Installation & Usage

1. Clone the repo:
    ```bash
    git clone https://github.com/your-username/heart-disease-classification.git
    cd heart-disease-classification
    ```

2. Install dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn fast-ml
    ```

3. Run the notebook:
    ```bash
    jupyter notebook HeartDisease_classification.ipynb
    ```

## 📊 Visualizations

- PCA scatter plots showing class separability
- Correlation heatmaps
- 3D plots for feature relationships
- Confusion matrices and dendrograms

## 📌 Conclusion

- **Naive Bayes** emerged as the top-performing model.
- **SVM** and **KNN** are competitive alternatives.
- **Decision Tree** showed relatively lower performance.

## 📬 Contact

For queries, please reach out to the project team members.

---

