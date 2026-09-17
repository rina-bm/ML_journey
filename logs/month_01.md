# 🧠 ML Journey

> **6-month intensive roadmap**
>
> **Month 1 — Classic Machine Learning Reboot**
>
> Цель месяца: восстановить базу классического ML, вернуть уверенную работу
> со sklearn и научиться самостоятельно собирать полный ML pipeline:
>
> `data → preprocessing → model → validation → metrics → interpretation`

---

## 📈 Progress

| Метрика                |    Прогресс |
| ---------------------- | ----------: |
| **Month**              |       1 / 6 |
| **Current block**      |       1 / 5 |
| **Completed**          | 0 / 30 days |
| **Progress**           |          0% |
| **Study time**         |          0h |
| **Target study time**  |   ~180–210h |
| **Projects completed** |       0 / 2 |

### Month progress

`░░░░░░░░░░░░░░░░░░░░ 0%`

---

# 🎯 Month Goal

К концу месяца я должен уметь:

- [ ] Определять тип ML-задачи: classification / regression / clustering
- [ ] Корректно разделять данные на train / validation / test
- [ ] Обрабатывать пропуски, категории и масштабирование
- [ ] Использовать `Pipeline` и `ColumnTransformer`
- [ ] Понимать и применять Logistic Regression
- [ ] Понимать Linear Regression, Ridge и Lasso
- [ ] Работать с KNN
- [ ] Работать с Decision Trees
- [ ] Работать с Random Forest
- [ ] Понимать bagging и boosting
- [ ] Использовать Gradient Boosting
- [ ] Понимать основы CatBoost / XGBoost
- [ ] Использовать SVM
- [ ] Понимать bias / variance
- [ ] Отличать overfitting от underfitting
- [ ] Выбирать подходящие classification metrics
- [ ] Выбирать подходящие regression metrics
- [ ] Работать с ROC-AUC
- [ ] Работать с PR / Recall / Precision / F1
- [ ] Подбирать classification threshold
- [ ] Понимать основы probability calibration
- [ ] Использовать Cross-Validation
- [ ] Использовать GridSearchCV / RandomizedSearchCV
- [ ] Выполнять feature engineering
- [ ] Понимать feature importance
- [ ] Использовать permutation importance
- [ ] Понимать основы SHAP
- [ ] Использовать KMeans / DBSCAN / Agglomerative Clustering
- [ ] Использовать PCA
- [ ] Объяснить, где может возникнуть data leakage
- [ ] Собрать sklearn pipeline с нуля без подсказки

---

# ✅ Definition of Done

День считается **завершённым**, только если:

- [ ] Теория по теме изучена / повторена
- [ ] Есть собственный код
- [ ] Код запущен и проверен
- [ ] Есть хотя бы один эксперимент или сравнение
- [ ] Записан короткий вывод
- [ ] Сделан commit
- [ ] Я могу объяснить тему своими словами

---

# 📚 Roadmap

## 📅 Block 1 — Classification Fundamentals

### Days 1–7

| День  | Тема                      | Статус | Время | Результат                                    |
| ----- | ------------------------- | :----: | :---: | -------------------------------------------- |
| Day 1 | ML Basics & Task Framing  |   ✅   |   —   | Определить target/features/task + train/test |
| Day 2 | Data Preprocessing        |   ⬜   |   —   | Imputer + OneHot + Scaling                   |
| Day 3 | Logistic Regression       |   ⬜   |   —   | LogisticRegression baseline                  |
| Day 4 | Classification Metrics    |   ⬜   |   —   | Accuracy / Precision / Recall / F1           |
| Day 5 | ROC-AUC & Threshold       |   ⬜   |   —   | ROC curve + threshold tuning                 |
| Day 6 | Multiclass Classification |   ⬜   |   —   | Macro/Micro F1 + OVR                         |
| Day 7 | Review + Mini Project     |   ⬜   |   —   | Classification mini-project                  |

### 🎯 Block Goal

- [ ] Понимать classification pipeline
- [ ] Уметь обучить Logistic Regression
- [ ] Понимать confusion matrix
- [ ] Отличать Precision от Recall
- [ ] Понимать F1
- [ ] Понимать ROC-AUC
- [ ] Уметь изменять classification threshold
- [ ] Понимать, почему accuracy может вводить в заблуждение

---

## 📅 Block 2 — Regression, KNN & Trees

### Days 8–14

| День   | Тема               | Статус | Время | Результат                         |
| ------ | ------------------ | :----: | :---: | --------------------------------- |
| Day 8  | Linear Regression  |   ⬜   |   —   | LinearRegression                  |
| Day 9  | Regression Metrics |   ⬜   |   —   | MAE / MSE / RMSE / R²             |
| Day 10 | Ridge & Lasso      |   ⬜   |   —   | Сравнение коэффициентов           |
| Day 11 | KNN                |   ⬜   |   —   | KNN Classifier + Regressor        |
| Day 12 | KNN & Scaling      |   ⬜   |   —   | Эксперимент scaling vs no scaling |
| Day 13 | Decision Trees     |   ⬜   |   —   | Trees с разной max_depth          |
| Day 14 | Bias / Variance    |   ⬜   |   —   | Train/Test comparison             |

### 🎯 Block Goal

- [ ] Понимать Linear Regression
- [ ] Отличать MAE / MSE / RMSE
- [ ] Понимать R²
- [ ] Объяснить Ridge
- [ ] Объяснить Lasso
- [ ] Понимать принцип KNN
- [ ] Объяснить curse of dimensionality
- [ ] Понимать устройство Decision Tree
- [ ] Отличать underfitting от overfitting
- [ ] Понимать bias-variance tradeoff

---

## 📅 Block 3 — Ensembles & Production-style sklearn

### Days 15–21

| День   | Тема                          | Статус | Время | Результат                              |
| ------ | ----------------------------- | :----: | :---: | -------------------------------------- |
| Day 15 | Bagging & Random Forest       |   ⬜   |   —   | RF vs Decision Tree                    |
| Day 16 | Stacking & Feature Importance |   ⬜   |   —   | Feature importance                     |
| Day 17 | Boosting                      |   ⬜   |   —   | Gradient Boosting / CatBoost / XGBoost |
| Day 18 | SVM & Kernels                 |   ⬜   |   —   | Linear vs RBF SVM                      |
| Day 19 | Feature Engineering           |   ⬜   |   —   | 5–10 новых признаков                   |
| Day 20 | Pipeline & ColumnTransformer  |   ⬜   |   —   | End-to-end Pipeline                    |
| Day 21 | Cross-Validation & Tuning     |   ⬜   |   —   | CV + Grid/Random Search                |

### 🎯 Block Goal

- [ ] Понимать bagging
- [ ] Понимать Random Forest
- [ ] Понимать boosting
- [ ] Отличать Random Forest от Gradient Boosting
- [ ] Понимать базовую идею stacking
- [ ] Понимать SVM
- [ ] Понимать kernel trick на интуитивном уровне
- [ ] Создавать новые признаки
- [ ] Использовать ColumnTransformer
- [ ] Использовать Pipeline
- [ ] Использовать Cross-Validation
- [ ] Настраивать гиперпараметры

---

## 📅 Block 4 — Titanic + Unsupervised ML

### Days 22–27

| День   | Тема                      | Статус | Время | Результат                      |
| ------ | ------------------------- | :----: | :---: | ------------------------------ |
| Day 22 | Titanic: EDA & Baseline   |   ⬜   |   —   | Logistic Regression baseline   |
| Day 23 | Titanic: Model Comparison |   ⬜   |   —   | LR / Tree / RF + CV            |
| Day 24 | Titanic: Evaluation       |   ⬜   |   —   | F1 / ROC-AUC / Error Analysis  |
| Day 25 | Clustering                |   ⬜   |   —   | KMeans / Hierarchical / DBSCAN |
| Day 26 | Clustering Metrics        |   ⬜   |   —   | Silhouette / ARI / NMI         |
| Day 27 | PCA & LDA                 |   ⬜   |   —   | PCA visualization              |

### 🎯 Block Goal

- [ ] Провести EDA реального датасета
- [ ] Построить baseline
- [ ] Сравнить несколько моделей честно
- [ ] Сделать CV
- [ ] Провести error analysis
- [ ] Понимать KMeans
- [ ] Понимать DBSCAN
- [ ] Понимать Hierarchical Clustering
- [ ] Использовать silhouette score
- [ ] Понимать PCA
- [ ] Понимать отличие PCA от feature selection

---

## 📅 Block 5 — Regression Project & Interpretability

### Days 28–30

| День   | Тема                            | Статус | Время | Результат                                |
| ------ | ------------------------------- | :----: | :---: | ---------------------------------------- |
| Day 28 | House Prices: Baseline          |   ⬜   |   —   | EDA + LinearRegression                   |
| Day 29 | House Prices: Improvements      |   ⬜   |   —   | Ridge / Lasso / RF + Feature Engineering |
| Day 30 | Interpretability & Month Review |   ⬜   |   —   | Importance + SHAP + Final Report         |

### 🎯 Block Goal

- [ ] Собрать regression pipeline
- [ ] Сравнить Linear / Ridge / Lasso / RF
- [ ] Сделать feature engineering
- [ ] Сравнить MAE / RMSE / R²
- [ ] Использовать permutation importance
- [ ] Понимать базовую идею SHAP
- [ ] Провести error analysis
- [ ] Оформить итоговый README проекта

---

# 🧪 Projects

## Project 1 — Titanic Classification

**Status:** ⬜

**Goal:** построить полный classification pipeline.

### Checklist

- [ ] EDA
- [ ] Missing values
- [ ] Encoding
- [ ] Train/test split
- [ ] Logistic Regression baseline
- [ ] Decision Tree
- [ ] Random Forest
- [ ] Cross-validation
- [ ] F1
- [ ] ROC-AUC
- [ ] Confusion Matrix
- [ ] Error Analysis
- [ ] README
- [ ] Final commit

---

## Project 2 — House Price Prediction

**Status:** ⬜

**Goal:** построить полный regression pipeline.

### Checklist

- [ ] EDA
- [ ] Data cleaning
- [ ] Feature engineering
- [ ] Linear Regression baseline
- [ ] Ridge
- [ ] Lasso
- [ ] Random Forest
- [ ] MAE
- [ ] RMSE
- [ ] R²
- [ ] Feature Importance
- [ ] Permutation Importance
- [ ] SHAP basics
- [ ] Error Analysis
- [ ] README
- [ ] Final commit

---

# 📝 Study Log

## Day 1

**Topic:** ML Basics

**Time:** —

### Completed

- [ ] Повторены classification / regression / clustering
- [ ] Выбран датасет
- [ ] Определён target
- [ ] Определены features
- [ ] Выполнен train/test split
- [ ] Сделан commit

### What I learned

-

### Problems / Questions

-

### Notes for review

- ***

## Day 2

**Topic:** Data Preprocessing

**Time:** —

### Completed

- [ ] `isna()`
- [ ] `fillna()`
- [ ] `SimpleImputer`
- [ ] `OneHotEncoder`
- [ ] `StandardScaler`
- [ ] Сделан мини-конспект
- [ ] Сделан commit

### What I learned

-

### Problems / Questions

-

### Notes for review

- ***

# 🔄 Review Queue

Темы, которые требуют повторения:

| Тема | Причина | Когда повторить | Статус |
| ---- | ------- | --------------- | :----: |
| —    | —       | —               |   —    |

---

# ⚠️ Backlog

Перенесённые или частично выполненные задачи:

| Задача | Причина | Новый срок |
| ------ | ------- | ---------- |
| —      | —       | —          |

---

# 🧠 Mistakes & Lessons

Здесь фиксируются **не просто ошибки кода**, а ошибки понимания.

| Ошибка | Почему произошла | Правильный подход |
| ------ | ---------------- | ----------------- |
| —      | —                | —                 |

---

# ⏱️ Study Time

| Block                    |   Time |
| ------------------------ | -----: |
| Classification           |     0h |
| Regression / KNN / Trees |     0h |
| Ensembles / Pipeline     |     0h |
| Unsupervised ML          |     0h |
| Projects                 |     0h |
| **Total**                | **0h** |

---

# 🏁 Month 1 Gate

Месяц считается действительно завершённым, если я могу **без пошаговой инструкции**:

- [ ] Загрузить табличные данные
- [ ] Провести базовый EDA
- [ ] Определить target и features
- [ ] Выбрать правильный split
- [ ] Найти потенциальный leakage
- [ ] Создать preprocessing
- [ ] Создать `ColumnTransformer`
- [ ] Создать `Pipeline`
- [ ] Обучить baseline
- [ ] Сравнить несколько моделей
- [ ] Использовать Cross-Validation
- [ ] Выбрать подходящую метрику
- [ ] Настроить threshold
- [ ] Выполнить базовый hyperparameter tuning
- [ ] Провести error analysis
- [ ] Интерпретировать результат модели
- [ ] Объяснить, почему финальная модель лучше baseline

---

# 📌 Month 1 Results

## Completed

- Days: **0 / 30**
- Study time: **0h**
- Projects: **0 / 2**

## Strong topics

-

## Weak topics

-

## Topics to repeat

-

## Main mistakes

-

## Best result

-

## What changes in Month 2

- ***

# 🎯 Current Focus

**Block 1 — Classification Fundamentals**

> Не просто вспомнить API sklearn, а восстановить понимание того,
> **что делает модель, почему выбирается конкретная метрика и где можно
> случайно получить нечестный результат.**
