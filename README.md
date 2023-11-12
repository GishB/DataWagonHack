# DataWagonHack

10 November 2023

#### Team: R5 (Rocket Five)
    - GishB https://github.com/GishB
    - geNaNaa https://github.com/geNaNaa
    - SergeyMatveev https://github.com/SergeyMatveev
    - maximdu https://github.com/maximdu

### Task №1 - PGK "Oracul":
    Main idea:
        Use Fourier time series decomposition to predict time series
    points at the future. It may be possible for stationary time series.
    By the way, it is intersting idea because we don`t need to train model
    in a supervised machine learning.

    Second idea:
        In case of some non-stationary time series we can try to
    use HoltWinter`s model with\or Fourier decomposition to increase
    regression score via boosting.

    Third idea:
        In case of some addition features like types of wagons or
    destination station, time of day and etc, we can try to use
    CatBoost model + Main or Second idea workflow.


#### EDA hints:
    pass

#### Workflow pipline:
    0. Check baseline
    1. Explotationary Data Analysis
    2. Transform data via T-SNE if applicable && EDA
    3. Check Fourier Model for default data
    4. Check HoltWinter`s Model for default data
    5. Check Boosting Model for default data
    6. Check CatBoost model for Transform data with boosting model
    7. Search for the best hyperparameters for ML models.

#### Results:
    The best score was achieved by using simple ```var.tail(3).mean()``` method.
