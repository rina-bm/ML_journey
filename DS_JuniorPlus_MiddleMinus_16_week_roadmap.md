# Data Scientist Junior+ / Middle-: интенсив 16 недель

**Цель.** За 12–16 недель при ранее изученной базе Python/ML подготовиться к техническим собеседованиям на Data Scientist Junior+ и отдельные Middle- вакансии. С 17-й недели — преимущественно собеседования, отклики и адресное закрытие пробелов.

**Основной профиль:** Applied / Product Data Science, табличный ML + SQL + статистика + A/B + бизнес-метрики. Этот профиль выбран вместо одновременной глубокой специализации в NLP, CV, RecSys и MLOps.

**Реалистичность:** 4 месяца по 6 дней в неделю, 6.5–8 продуктивных часов в день дают ~624–768 часов. Это достаточно для сильной практической подготовки при наличии основы, но не заменяет 1–3 года опыта, типичного для большинства Middle вакансий.

## Критерии приоритета

- **A, обязательно уверенно:** Python/pandas/NumPy, SQL/PostgreSQL, вероятности и статистика, проверка гипотез, A/B, EDA, классический ML, sklearn Pipeline, CatBoost/LightGBM, валидация/leakage, продуктовые метрики, воспроизводимые эксперименты, бизнес-интерпретация.
- **B, практическое владение:** Git, Docker, pytest, MLflow, FastAPI или batch inference, временные ряды, основы причинного анализа, data quality, PostgreSQL/DuckDB/Parquet, базовая визуализация/дашборд.
- **C, ориентир и мини-практика:** PyTorch, embeddings/LLM, ранжирование/RecSys, PySpark, Airflow, ClickHouse, CI/CD, облако. Углублять только под подходящие вакансии.

## Нагрузка

- 6 учебных дней в неделю, один выходной; 6–9 часов в день (целиться в 7–8 часов качественной работы, без учёта перерывов).
- Обычный день: 1.5 ч теория/математика, 1.5 ч SQL/статистика, 3–3.5 ч код/эксперименты, 0.5–1 ч разбор ошибок и заметки.
- Проектный день: 1 ч изучение необходимого, 5–6 ч работа над кейсом, 1 ч тесты/README/защита решения.
- Раз в неделю: 60–90 минут повторения и самопроверки; не растягивать непонятную тему на несколько дней без кода.

## Технологии и платформы

| Назначение | Основной выбор | Дополнительно |
|---|---|---|
| Среда и Git | VS Code, Jupyter, GitHub, venv/uv | Kaggle Notebooks, Colab |
| Python data | NumPy, pandas, scipy, matplotlib, seaborn, statsmodels | polars |
| SQL/data | PostgreSQL, DBeaver, DuckDB, Parquet | ClickHouse, PySpark |
| ML | scikit-learn, CatBoost, LightGBM | XGBoost, Optuna, imbalanced-learn |
| Эксперименты | scipy.stats, statsmodels, bootstrap | CUPED, DoWhy/uplift libraries |
| Интерпретация | permutation importance, SHAP | PDP/ALE |
| Визуализация | matplotlib/seaborn, Streamlit | Metabase/Power BI |
| Engineering | pytest, Git, Docker, FastAPI или batch | MLflow, GitHub Actions, Airflow |
| DL/AI | PyTorch, Hugging Face (базово) | RAG, RecSys frameworks |

## Обязательные результаты

1. **A/B / Product Analytics** — SQL-когортный анализ, план эксперимента, мощность, эффект/CI, продуктовое memo на реальном рандомизированном наборе.
2. **Business ML (Churn или Propensity)** — реальные табличные данные, baseline и CatBoost/LightGBM, честная validation strategy, интерпретация, решение по порогу.
3. **Специализированный кейс (forecasting / product causal / ranking)** — полноценное сравнение с baseline; честно отделять наблюдательные данные от рандомизированных.
4. **Capstone** — не новый четвёртый большой датасет обязательно: можно довести проект №2/№3 до SQL + train/predict + tests + Docker + monitoring design и business case.

**Правило:** никакой модели без baseline, никакого тюнинга на test, никакой «A/B-аналитики» по случайно выдуманным экспериментальным группам и никакого утверждения о причинности по одной корреляции.

## Детальный план: 16 недель / 96 учебных дней

### Неделя 01. Python / SQL / EDA и постановка DS-задачи

**Результат недели:** Найти проблему данных, собрать EDA и сделать первые сложные SQL-запросы.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 1 | Python/NumPy/pandas audit | pandas merge/groupby/transform, векторизация, типы, NaN | EDA одного набора, отчёт о дубликатах и пропусках |
| 2 | SQL: SELECT, JOIN, GROUP BY | кардинальность соединений, HAVING, NULL | 12 SQL-запросов в PostgreSQL + проверка дублей после JOIN |
| 3 | SQL: CTE, оконные функции | ROW_NUMBER, LAG/LEAD, SUM OVER, PARTITION BY | 8 задач на события пользователей, сессии и ранжирование |
| 4 | EDA и качество данных | bias отбора, leakage, выбросы, визуализация | 5 содержательных гипотез и графиков с выводами |
| 5 | Мат. база I | векторы/матрицы, производные, градиент, скалярное произведение | NumPy: расстояния, линейная модель и градиент на игрушечном примере |
| 6 | Мини-кейс и самопроверка | task framing: target, объект, baseline, бизнес-метрика | SQL -> pandas -> EDA -> 1-страничный brief, commit |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 02. Теория вероятностей и статистика

**Результат недели:** Уметь рассуждать об оценках, разбросе и неопределённости.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 7 | Вероятности | условная вероятность, Байес, независимость, Bernoulli/Binomial | 10 задач + симуляция условных вероятностей в NumPy |
| 8 | Распределения | Normal, Bernoulli, Binomial, Poisson, экспоненциальное | SciPy: 4 распределения, выборки и графики |
| 9 | Описательная статистика | выборка/генеральная совокупность, медиана, дисперсия, ковариация | бутстрэп среднего/медианы и сравнение оценок |
| 10 | CLT и доверительные интервалы | стандартная ошибка, закон больших чисел, интерпретация CI | симуляция покрытия 95% CI при повторных выборках |
| 11 | Тесты гипотез | H0/H1, p-value, alpha, ошибки I/II рода, Welch t-test, chi-square | проверить 2 гипотезы в scipy.stats, сформулировать ограничения |
| 12 | Эффект и мощность | effect size, power, размер выборки, bootstrap/permutation | посчитать sample size и создать краткий stats-cheatsheet |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 03. Линейные модели и оценка качества

**Результат недели:** Восстановить supervised ML на уровне объяснения и кода.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 13 | ML pipeline и leakage | split train/val/test, strata, group/time, preprocessing внутри CV | осмысленный split и Dummy baseline на dataset |
| 14 | Линейная регрессия | OLS, коэффициенты, допущения, residuals | LinearRegression и residual plots; MAE/RMSE/R2 |
| 15 | Регуляризация | L1/L2, Ridge/Lasso, bias-variance, scaling | сравнение коэффициентов и CV на Ridge/Lasso |
| 16 | Логистическая регрессия | sigmoid/log-odds, logloss, C, class weights | LogReg и интерпретация коэффициентов после scaling |
| 17 | Классификационные метрики | confusion, P/R/F1, ROC-AUC, PR-AUC, threshold | метрики на balanced/imbalanced данных, threshold table |
| 18 | Многокласс и KNN/SVM | OvR, macro/micro; KNN; линейное/RBF ядро SVM | эксперимент: 3 модели, scaling, macro-F1 |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 04. Деревья, ансамбли, валидация

**Результат недели:** Собрать воспроизводимый классический ML baseline с CV.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 19 | Деревья решений | impurity, split, pruning, глубина, train-CV gap | визуализация дерева + learning curve |
| 20 | Random Forest и ExtraTrees | bootstrap, bagging, feature subsampling, OOB | сравнение дерева и ансамбля на одинаковых folds |
| 21 | Gradient Boosting | градиентный бустинг, learning rate, early stopping | HistGradientBoosting и CatBoost baseline |
| 22 | Пайплайны sklearn | SimpleImputer, OneHotEncoder, StandardScaler, ColumnTransformer | единый Pipeline для mixed-type data |
| 23 | CV и tuning | StratifiedKFold, GroupKFold, TimeSeriesSplit; RandomizedSearchCV | оптимизация 3 параметров без утечки |
| 24 | Gate месяца 1 | объяснение моделей, leakage, выбор метрик | с нуля за 2 часа pipeline + CV; 20 вопросов; README |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 05. SQL advanced + продуктовая аналитика

**Результат недели:** Уметь получать признаки из событий и измерять поведение пользователей.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 25 | PostgreSQL углублённо | индексы, EXPLAIN, оконные функции, подзапросы | 10 задач SQL с разбором плана 2 запросов |
| 26 | События и воронки | event schema, сессии, conversion, funnel | SQL funnel от просмотра до покупки; корректные denominator |
| 27 | Retention и когорты | D1/D7/D30, cohort table, активность | когортная матрица retention в SQL + pandas |
| 28 | Unit economics | ARPU, ARPPU, AOV, LTV, CAC, churn | metrics dictionary и расчёт метрик из event data |
| 29 | Визуализация и коммуникация | сложные графики, сегменты, ограничения | Streamlit или Metabase: 1 dashboard с выводами |
| 30 | Product case | что улучшить и как измерить | 5 гипотез, guardrail metrics, SQL notebook и memo |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 06. A/B-тестирование и дизайн экспериментов

**Результат недели:** От бизнес-гипотезы прийти к корректному решению об эффекте.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 31 | Дизайн A/B | рандомизация, unit of randomization, SRM, guardrail | написать experiment design до чтения результатов |
| 32 | Ключевые метрики | ratio metrics, conversion, outliers, distributions | SQL расчёт по участникам, sanity checks |
| 33 | Статистический анализ | Welch t, z/chi-square, bootstrap, CI, uplift | A/B notebook с p-value, CI и практической значимостью |
| 34 | Power и множественные тесты | MDE, sample size, Bonferroni/BH, peeking | калькулятор мощности и анализ 3 метрик |
| 35 | CUPED и variance reduction | pre-experiment covariate, CUPED, проблемы смешения | симуляция CUPED; сравнить ширину доверительных интервалов |
| 36 | A/B project v1 | реальный рандомизированный dataset, отчёт для продукта | полный кейс A/B: data -> SQL -> test -> decision |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 07. Advanced tabular ML

**Результат недели:** Перейти от учебных моделей к качественному DS-эксперименту.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 37 | CatBoost | cat features, ordered boosting, early stopping | CatBoost classifier + baseline сравнение |
| 38 | LightGBM / XGBoost | деревья, листья, subsample, regularization | 2 бустинга + ограниченный поиск параметров |
| 39 | Дисбаланс | PR-AUC, cost matrix, class_weight, SMOTE внутри CV | обучение/сравнение с безопасным resampling |
| 40 | Feature engineering/selection | агрегаты, target encoding leakage, ablation | 5-10 фичей + абляция по CV |
| 41 | SHAP и интерпретация | permutation importance, global/local SHAP, корреляции | summary + 3 локальных объяснения и ограничения |
| 42 | Ошибки и калибровка | error slicing, calibration, Brier score | сегменты с ошибками, threshold и calibration report |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 08. Большой проект № 1: Churn / Propensity

**Результат недели:** Один полноценный бизнес-ориентированный табличный ML-кейс.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 43 | Problem framing | business KPI, prediction horizon, time of decision | brief: цель, целевая переменная, метрики, стоимость ошибок |
| 44 | Данные и SQL-фичи | SQL extraction, cohort leakage, temporal correctness | витрина фичей + data quality report |
| 45 | Baseline и CV | логрег/RandomForest, split strategy, baseline | воспроизводимое обучение и результаты baseline |
| 46 | Boosting и эксперименты | CatBoost/LightGBM, tuning budget, MLflow optional | best candidate + журнал 5 экспериментов |
| 47 | Decision layer | threshold, calibration, expected effect, error analysis | report + интерпретация + ограничения |
| 48 | Defense & Gate месяца 2 | code review, тесты, README, бизнес-решение | demo 7 минут и ответы на 20 вопросов |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 09. Временные ряды

**Результат недели:** Уметь корректно валидировать и прогнозировать во времени.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 49 | Time-series EDA | trend, seasonality, frequency, missing timestamps | EDA временного ряда без утечки |
| 50 | Baselines и метрики | naive/seasonal naive, MAE, WAPE, MASE | 3 baseline + честное сравнение |
| 51 | Time-based validation | rolling origin, horizon, look-ahead leakage | функция backtesting и график по folds |
| 52 | Features для прогноза | lags, rolling, holidays, calendar, covariates | lag/rolling features, обучить CatBoost/LightGBM |
| 53 | ETS / ARIMA обзор | стационарность, ACF/PACF, statsmodels | одна классическая модель и её ограничения |
| 54 | Мини-проект forecasting | прогноз спроса/продаж, бизнес-ошибки | README с backtest, baseline и forecast plot |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 10. Data Engineering для DS

**Результат недели:** Понимать источники, витрины и воспроизводимые пайплайны.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 55 | DB и DWH | OLTP/OLAP, star schema, fact/dimension, grain | нарисовать схему мини-хранилища для ML |
| 56 | PostgreSQL -> feature mart | SQL моделирование витрины и контроль качества | SQL pipeline с материализацией признаков |
| 57 | Parquet и DuckDB | columnar, Arrow, parquet partition | прочитать/записать parquet; SQL-проход DuckDB |
| 58 | PySpark основы | DataFrame API, Spark SQL, lazy execution | ETL с агрегатами на локальном Spark; explain физического плана |
| 59 | Airflow концепции | DAG, retries, scheduling, backfill | минимальный локальный DAG или эквивалентный сценарий |
| 60 | Контроль DQ | schema drift, проверка дубликатов/NULL/ranges | pytest + 5 data quality checks |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 11. DL минимум + современный стек

**Результат недели:** Понимать нейросети, не превращая подготовку в четыре специализации.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 61 | PyTorch tensors/autograd | tensor, device, loss, gradient, optimizer | маленький regression/classification training loop |
| 62 | nn.Module/DataLoader | MLP, batches, train/eval, checkpoints | одна NN с train/val метриками |
| 63 | DL vs CatBoost | сравнение на одинаковой табличной задаче | результат сравнения с объяснением стоимости |
| 64 | NLP/LLM основы | embeddings, Transformer, fine-tuning vs RAG | text classifier на готовых embeddings или обзор RAG |
| 65 | RecSys/ranking основы | implicit feedback, ranking metrics, cold start | popularity baseline + Recall@K/NDCG@K toy case |
| 66 | Выбор специализации | time series vs product DS vs recommendation/NLP | одностраничный memo: что углублять и что пока пропустить |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 12. Causal inference + второй прикладной кейс

**Результат недели:** Уметь распознавать причинные ловушки и защитить решение.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 67 | Причинность | корреляция vs причина, confounders, collider | нарисовать 3 простых DAG и выявить bias |
| 68 | Квазиэксперименты | difference-in-differences, matching, assumptions | toy DiD с проверкой parallel trends |
| 69 | Uplift modeling обзор | treatment, CATE, T/S-learners, AUUC/Qini идея | простое uplift-baseline только при наличии treatment data |
| 70 | Второй кейс выбор | forecasting ИЛИ retention/A-B/cause ИЛИ ranking | scope, datasets, цели и метрики |
| 71 | Моделирование и проверка | честный split, baseline, 1 улучшение | работающий второй кейс и error analysis |
| 72 | Gate месяца 3 | защита SQL, статистики, модели, бизнеса | 2 коротких mock; решение: идти на 3-месячный рынок или на 4-й месяц |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 13. Capstone: бизнес-задача и архитектура

**Результат недели:** Подготовить сильный end-to-end DS проект для портфолио.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 73 | Бизнес-проблема | стейкхолдер, решение, KPI, ограничения | 1-page project brief с baseline |
| 74 | Данные и схема | источники, лицензии, quality checks, DWH/SQL | data dictionary и воспроизводимая загрузка |
| 75 | SQL-витрина | JOIN keys, as-of features, time consistency | скрипт подготовки витрины на SQL |
| 76 | EDA и риски | сегменты, outliers, leakage, fairness/context | EDA из 5 полезных выводов |
| 77 | Дизайн валидации | time/group split, business metric, holdout | validation protocol до тюнинга |
| 78 | Кодовая структура | src/, notebooks/, tests/, config, README | рабочий skeleton и baseline |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 14. Capstone: эксперимент и бизнес-вывод

**Результат недели:** Сделать модель и доказать полезность на честных метриках.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 79 | Baseline и обучение | Dummy/линейная + бустинг, reproducible seed | baseline + 2 candidates |
| 80 | Hyperparameter tuning | Optuna/RandomizedSearchCV, trial tracking | только 10-30 осмысленных trials |
| 81 | Interpretability | SHAP/permutation, uncertainty, errors | отчёт по важности и сегментам ошибок |
| 82 | Business evaluation | cost matrix, lift, threshold, KPI estimate | численный бизнес-кейс с допущениями |
| 83 | Эксперименты / A/B plan | можно ли рандомизировать и что измерять | экспериментальный план с guardrails + MDE |
| 84 | Reproducibility | seed, experiment log, versioned data/model | полное воспроизводимое обучение на clean env |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 15. DS Engineering минимум

**Результат недели:** Проект должен быть запускаемым и проверяемым, а не только ноутбуком.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 85 | Python package | typing, functions, pathlib, configs, logging | train.py, predict.py, pyproject или requirements |
| 86 | pytest | unit tests, fixtures, edge cases | не менее 8 содержательных тестов |
| 87 | MLflow / artifacts | experiment tracking, model version metadata | записать метрики и артефакт модели |
| 88 | FastAPI или batch | Pydantic schema, /predict или batch predict | запуск предсказаний без Jupyter |
| 89 | Docker и CI basics | Dockerfile, GitHub Actions, fresh clone | docker run + тесты в CI (по возможности) |
| 90 | Мониторинг | input drift, data quality, performance, retraining | monitoring memo с 5 сигналами и ограничениями |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.

### Неделя 16. Проверка уровня и выход на рынок

**Результат недели:** Защитить портфолио и убрать оставшиеся критические пробелы.

| День | Фокус | Что разобраться | Практический результат |
|---:|---|---|---|
| 91 | QA портфолио | README, case study, reproducibility, licenses | 2 сильных проекта + 1 компактный кейс |
| 92 | SQL timed | JOIN/CTE/windows/retention/cohort | 10 задач за 90 мин с проверкой |
| 93 | Statistics + A/B timed | CI/p-value/power/CUPED/SRM/ratio metrics | 8 прикладных сценариев под таймер |
| 94 | ML + case interview | split/leakage/boosting/time series/metrics | объяснить модель и business case у доски |
| 95 | Python + code review | pandas, functions, pytest, debugging | рефакторинг кода и исправление трёх ошибок |
| 96 | Gate месяца 4 | project defense + mock interview + gap closure | readiness checklist, CV, GitHub, 20 целевых вакансий |

**День 7:** отдых или максимум 60 минут лёгкого повторения; не считать новым учебным днём.


## Gates готовности

| Срок | Нужно уметь без пошаговых подсказок |
|---|---|
| 4 недели | SQL с CTE/windows, доверительный интервал и p-value, классификация/регрессия, CatBoost + sklearn Pipeline + CV, выбор метрики и объяснение leakage |
| 8 недель | Спроектировать/разобрать A/B с CI/power/SRM, собрать продуктовые метрики в SQL, получить сильный tabular baseline и осмысленный бизнес-вывод |
| 12 недель | Провести time-series backtest, объяснить data mart/ETL, дать causality caveats и защитить 2 законченных DS кейса; возможный старт интервью Junior+ |
| 16 недель | 2 сильных воспроизводимых проекта, 1 аналитический/A-B кейс, тесты и inference, 90-минутный SQL mock, ML/statistics case interview, резюме/портфолио |

## Сокращение до 12 недель

**Если срок ровно три месяца:** обязательные недели 1–9, 12 и проекты оставляем; в 10–11 неделях изучить только SQL-витрины, Parquet, минимальный PyTorch обзор за 1–2 дня; в 12-ю неделю закончить один главный проект и A/B report. Airflow, Spark, RecSys, NLP, Docker/CI углублённо откладываются под конкретные вакансии. Не сокращать статистику, SQL, валидацию, A/B и честную проектную практику. Ожидание: скорее Junior/Junior+, а не Middle-.

## После обучения: 4 недели собеседований

- Неделя 17: целевые отклики, скрининги, ежедневные SQL+Python drills, one-pager по ML/статистике.
- Неделя 18: A/B и case interviews, статистика под таймер, защита бизнес-кейса.
- Неделя 19: ML/Applied DS интервью, практика задач по feature leakage, метрикам, бустингу, временным рядам.
- Неделя 20: интервью, исправление выявленных ошибок, точечная адаптация портфолио под тип вакансий. Продолжать отклики, а не ждать идеального готового состояния.

## Источники

- Актуальная вакансия МТС Банк: https://career.habr.com/vacancies/1000167271
- Актуальная Middle-вакансия BETBOOM: https://career.habr.com/vacancies/1000168794
- Обзор обязанностей уровней DS, Хабр Карьера: https://career.habr.com/professions/data-scientist
- scikit-learn guide: https://scikit-learn.org/stable/user_guide.html
- PostgreSQL docs: https://www.postgresql.org/docs/current/tutorial-sql.html
- SciPy statistics: https://docs.scipy.org/doc/scipy/reference/stats.html
- statsmodels: https://www.statsmodels.org/stable/index.html
- CatBoost docs: https://catboost.ai/en/docs/
- PyTorch tutorials: https://docs.pytorch.org/tutorials/
