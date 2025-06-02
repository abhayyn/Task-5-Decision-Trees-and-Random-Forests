**Task 5: Decision Trees and Random Forests**

#  Task 5: Decision Trees and Random Forests

This project is part of the **AI & ML Internship** and focuses on understanding and implementing tree-based machine learning models — specifically Decision Trees and Random Forests — using the **Heart Disease Dataset**.

##  Objectives

* Implement a **Decision Tree Classifier** and visualize its structure.
* Analyze **overfitting** and control tree complexity with hyperparameters like `max_depth`.
* Implement a **Random Forest Classifier** and compare its performance.
* Visualize and interpret **feature importances**.
* Evaluate models using **cross-validation** for reliability.


## Tools & Libraries

* Python
* Scikit-learn
* Pandas, NumPy
* Matplotlib, Seaborn
* Graphviz or `plot_tree` from Scikit-learn


##  Dataset

* **Name**: Heart Disease Dataset
* **Source**: [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
* **Target Column**: `target` (1 = disease, 0 = no disease)


##  Steps Implemented

###  1. Load & Preprocess Data

* Loaded dataset using pandas
* Handled features and target separation
* Standardized features using `StandardScaler`

###  2. Train a Decision Tree

* Used `DecisionTreeClassifier`
* Visualized tree using `plot_tree`
* Accuracy evaluated on test data

###  3. Control Overfitting

* Limited tree depth using `max_depth=3`
* Compared performance with unpruned tree

###  4. Train a Random Forest

* Used `RandomForestClassifier` with 100 trees
* Higher accuracy and generalization compared to a single tree

###  5. Feature Importance

* Used `.feature_importances_` to identify key predictors
* Visualized using `Seaborn` barplot

###  6. Cross-Validation

* Used `cross_val_score` with 5 folds
* Calculated average model performance across splits

##  Results

| Model             | Accuracy (Test) | Cross-Validation Avg |
| ----------------- | --------------- | -------------------- |
| Decision Tree     | \~82%           | \~78%                |
| Pruned Tree (d=3) | \~79%           | \~75%                |
| Random Forest     | \~87%           | \~84%                |


##  Files in Repository

* `task5_decision_tree_random_forest.ipynb` – Jupyter notebook with code and outputs
* `heart.csv` – Dataset used
* `README.md` – Project overview and explanations
* `screenshot` – plot created using python



